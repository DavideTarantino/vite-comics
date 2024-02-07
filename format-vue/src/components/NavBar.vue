<script>
    export default{
        name: 'NavBar',
        data(){
            return{
                cta: [
                    {
                        name: 'characters',
                        current: false
                    },
                    {
                        name: 'comics',
                        current: true
                    },
                    {
                        name: 'movies',
                        current: false
                    },
                    {
                        name: 'tv',
                        current: false
                    },
                    {
                        name: 'games',
                        current: false
                    },
                    {
                        name: 'collectibles',
                        current: false
                    },
                    {
                        name: 'videos',
                        current: false
                    },
                    {
                        name: 'fans',
                        current: false
                    },
                    {
                        name: 'news',
                        current: false
                    },
                    {
                        name: 'shop',
                        current: false
                    }
                ]
            }
        }
    }
</script>

<template>
    <main>
        <figure>
            <img src="../img/dc-logo.png" alt="logo">
        </figure>
            <ul>
                <li :class=" element.current ? 'active' : '' " v-for="(element,index) in cta">{{ element.name }}</li>
            </ul>
    </main>
</template>

<style lang="scss" scoped>
@use '../assets/partials/mixins' as *;

    main{
        @include page-layout;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1%;

        img{
            width: 80%;
        }

        ul{
            display: flex;
            gap: 30px;

            li{
                text-transform: uppercase;
                font-family: sans-serif;
                font-size: 80%;
            }
        }
    }

    .active{
        color: blue;
    }
</style>
