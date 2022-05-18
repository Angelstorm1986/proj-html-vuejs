<template>
    <main>
        <app-jumbotron/>
        <app-specialist/>
        <app-results/>
        <app-explore/>
        <app-core/>
        <app-home/>
        <app-news/>
        <app-partners/>
    </main>
</template>

<script>
import AppJumbotron from './AppJumbotron.vue'
import AppSpecialist from './AppSpecialist.vue'
import AppResults from './AppResults.vue'
import AppExplore from './AppExplore.vue'
import AppCore from './AppCore.vue'
import AppHome from './AppHome.vue'
import AppNews from './AppNews.vue'
import AppPartners from './AppPartners.vue'
export default {
    name: 'AppMain',
    components:{
        AppJumbotron,
        AppSpecialist,
        AppResults,
        AppExplore,
        AppCore,
        AppHome,
        AppNews,
        AppPartners
    }
}
</script>

<style lang="scss">
@import '../style/vars';
</style>