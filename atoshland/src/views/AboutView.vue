<template>
  <div class="justify-center flex bg-green-300 items-center h-screen">
    <div class="text-4xl">
      <p>{{ $t('message.change') }}</p>
      <Hello18nComponent></Hello18nComponent>
    </div>
  </div>
</template>

<script>
import  Hello18nComponent from '../components/HelloI18n'

export default {
  components: {
    Hello18nComponent
  }
}
</script>
