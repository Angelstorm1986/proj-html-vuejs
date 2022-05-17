<template>
    <main>
        <app-jumbotron/>
        <app-partners/>
    </main>
</template>

<script>
import AppJumbotron from './AppJumbotron.vue'
import AppPartners from './AppPartners.vue'
export default {
    name: 'AppMain',
    components:{
        AppJumbotron,
        AppPartners
    }
}
</script>

<style lang="scss">
@import '../style/vars';
</style>