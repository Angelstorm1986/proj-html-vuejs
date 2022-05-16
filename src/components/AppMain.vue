<template>
  <main>
      <app-jumbotron/>
  </main>
</template>

<script>
import AppJumbotron from './AppJumbotron.vue'
export default {
    name: 'AppMain',
    components:{
        AppJumbotron
    }
}
</script>

<style lang="scss">
@import '../style/vars';
</style>