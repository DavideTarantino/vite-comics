<script>
    export default{
        name: 'CallToAction',
        data(){
            return{
               
            }
        }
    }
</script>

<template>
    <main>
        <section>
            <div>
                <img src="../img/buy-comics-digital-comics.png">
                <h4>Digital comics</h4>
            </div>
            <div>
                <img src="../img/buy-comics-merchandise.png">
                <h4>DC merchandaise</h4>
            </div>
            <div>
                <img src="../img/buy-comics-subscriptions.png">
                <h4>subscription</h4>
            </div>
            <div>
                <img src="../img/buy-comics-shop-locator.png">
                <h4>Comic shop location</h4>
            </div>
            <div>
                <img src="../img/buy-dc-power-visa.svg">
                <h4>dc power visa</h4>                
            </div>
        </section>
    </main>
</template>

<style lang="scss" scoped>
@use '../assets/partials/mixins' as *;

main{
    background-color: #0282F9;
    
    section{
        @include page-layout;
        padding: 2%;
        display: flex;
        justify-content: center;
        gap: 5%;

        div{
            display: flex;
            align-items: center;
            gap: 3%;
            color: white;
            text-transform: uppercase;

            img{
                width: 50px;
            }
        }
    }
}
</style>