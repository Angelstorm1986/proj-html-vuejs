<template>
    <main>
        <app-jumbotron/>
        <app-home/>
        <app-news/>
        <app-partners/>
    </main>
</template>

<script>
import AppJumbotron from './AppJumbotron.vue'
import AppHome from './AppHome.vue'
import AppNews from './AppNews.vue'
import AppPartners from './AppPartners.vue'
export default {
    name: 'AppMain',
    components:{
        AppJumbotron,
        AppHome,
        AppNews,
        AppPartners
    }
}
</script>

<style lang="scss">
@import '../style/vars';
</style>