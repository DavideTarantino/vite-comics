<script>
    import NavBar from './components/NavBar.vue'
    import NewContent from './components/NewContent.vue'
    import CallToAction from './components/CallToAction.vue'
    import MainSection from './components/MainSection.vue'

    export default {
        components: {
            NavBar,
            NewContent,
            CallToAction,
            MainSection
        }
    }
</script>

<template>
    <NavBar/>

    <NewContent/>

    <CallToAction/>

    <MainSection/>
</template>

<style lang="scss">
    @use './assets/style.scss'
</style>
