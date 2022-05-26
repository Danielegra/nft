<template>
  <div class="justify-center flex bg-yellow-300 items-center h-screen">
    <div class="text-4xl">
      <p>{{ $t('message.welcome') }}</p> ✌️🤟🤘
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src
import '../styles/app.css'

@Options({
  components: {
    HelloWorld,
  },
})
export default class HomeView extends Vue {}
</script>
