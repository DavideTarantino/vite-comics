<script>
    import NavBar from './components/NavBar.vue'
    import NewContent from './components/NewContent.vue'
    import CallToAction from './components/CallToAction.vue'
    import MainSection from './components/MainSection.vue'
    import SocialFooter from './components/SocialFooter.vue'

    export default {
        components: {
            NavBar,
            NewContent,
            CallToAction,
            MainSection,
            SocialFooter
        }
    }
</script>

<template>
    <NavBar/>

    <NewContent/>

    <CallToAction/>

    <MainSection/>

    <SocialFooter/>
</template>

<style lang="scss">
    @use './assets/style.scss'
</style>
