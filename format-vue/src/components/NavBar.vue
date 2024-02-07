<script>
    export default{
        data(){
            name: 'NavBar'
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
            <img src="../img/favicon.ico" alt="logo">
        </figure>
            <ul>
                <li :class=" element.current ? 'active' : '' " v-for="(element,index) in cta">{{ element.name }}</li>
            </ul>
    </main>
</template>

<style lang="scss">
    main{
        display: flex;
        justify-content: space-between;
        width: 70%;
        margin: 0 auto;
        padding: 1%;
        align-items: center;

        img{
            width: 150%;
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
