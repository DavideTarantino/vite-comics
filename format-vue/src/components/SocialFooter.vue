<script>
    export default{
        name: 'SocialFooter',
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
            <button type="button">SIGN-UP NOW!</button>
        </div>
        <div id="imgs">
            <h3>FOLLOW US</h3>
            <img src="../img/footer-facebook.png" alt="facebook">
            <img src="../img/footer-twitter.png" alt="twitter">
            <img src="../img/footer-youtube.png" alt="YouTube">
            <img src="../img/footer-pinterest.png" alt="Pinterest">
            <img src="../img/footer-periscope.png" alt="Periscope">
        </div>
    </section>
</main>
</template>

<style lang="scss" scoped>
@use '../assets/partials/mixins' as *;

main{
    background-color: #303030;

    section{
        @include page-layout;
        padding: 1%;
        color: white;
        display: flex;
        justify-content: space-between;

        button{
            padding: 10%;
            width: 130px;
            border: 2px solid blue;
            color: white;
            background-color: #303030;
        }

        #imgs{
            display: flex;
            gap: 3%;
            align-items: center;
            

            h3{
              width: 190px;
              color: cyan;  
            }
        }
    }
}

</style>