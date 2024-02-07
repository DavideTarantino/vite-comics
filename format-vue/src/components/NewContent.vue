<script>
    export default{
        name: 'NewContent',
        data(){
            return{
               
            }
        }
    }
</script>

<template>
<main>
    <section>
        <h3>Content Goes Here</h3>
    </section>
</main>
</template>

<style lang="scss" scoped>
@use '../assets/partials/mixins' as *;

main{
    background-color: black;

    section{
        @include page-layout;
        padding: 2%;
        color: white;
    }
}

</style>
