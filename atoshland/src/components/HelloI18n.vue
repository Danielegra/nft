<template>
  <select v-model="$i18n.locale">
    <option v-for="(locale, i) in locales" :key="`locale-${i}`" :value="locale" @click="switchLocale(locale)">
      {{ locale }}
    </option>
  </select>
  <p>{{ $t('message.test') }}</p>
  <p>{{ $i18n.locale }}</p>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'HelloI18n',
  data() {
    return { locales: ["it", "en"] };
  },
  methods: { // <---------------------------
    switchLocale(locale: any) {
      console.log(111, this.$i18n.locale)
      if (this.$i18n.locale !== locale) {
        this.$i18n.locale = locale;
      }
    }
  },
})
</script>
