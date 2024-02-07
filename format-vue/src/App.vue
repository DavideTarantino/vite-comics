<script>
    import NavBar from './components/NavBar.vue'
    import NewContent from './components/NewContent.vue'
    import CallToAction from './components/CallToAction.vue'

    export default {
        components: {
            NavBar,
            NewContent,
            CallToAction
        }
    }
</script>

<template>
    <NavBar/>

    <NewContent/>

    <CallToAction/>
</template>

<style lang="scss">
    @use './assets/style.scss'
</style>
