<script>
    export default{
        name: 'MainSection',
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
                <div>
                    <ul><h3>DC COMICS</h3>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                </div>
                <div>
                    <ul><h3>SHOP</h3>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
            </div>
            <div>
                <ul><h3>DC</h3>
                    <li>Terms Of Use</li>
                    <li>Privacy policy (New)</li>
                    <li>Ad Choiches</li>
                    <li>Advertising</li>
                    <li>Jobs</li>
                    <li>Subscription</li>
                    <li>Talent Workshops</li>
                    <li>CpsC Certificates</li>
                    <li>Ratings</li>
                    <li>Shop Help</li>
                    <li>Contact Us</li>
                </ul>
            </div>
            <div>
                <ul><h3>SITES</h3>
                    <li>DC</li>
                    <li>MAD Magazine</li>
                    <li>DC Kids</li>
                    <li>DC Universe</li>
                    <li>DC Power Visa</li>
                </ul>
            </div>
        <img src="../img/dc-logo-bg.png">      
    </section>
</main>
</template>

<style lang="scss" scoped>
@use '../assets/partials/mixins' as *;

main{
    background-image: url(../img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    height: 50vh;

    section{
        @include page-layout;
        display: flex;
        gap: 5%;
        color: white;
        padding-block: 4%;
        line-height: 150%;
        position: relative;

        img{
            position: absolute;
            right: 0px;
            top: -50px;
        }

        h3{
            padding-bottom: 7%;
        }

        >div{
            display: flex;
            flex-direction: column;
            gap: 30px;
        }
    }
}

</style>