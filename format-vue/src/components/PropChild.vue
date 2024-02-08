<script>
export default{
    name: 'PropChild',
    props: {
        propsThumbs: String,
        propsTitolo: String
    }
}
</script>

<template>
    <div>
        <figure>
            <img :src="propsThumbs" alt="">
        </figure>
        <h4>{{ propsTitolo }}</h4>
    </div>
</template>

<style lang="scss" scoped>
    div{
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;

            h4{
                max-width: 180px;
            }
        }

        img{
            width: 160px;
            object-fit: cover;
        }
</style>
