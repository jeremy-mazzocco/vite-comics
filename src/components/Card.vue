<script>
export default {
    name: "Card",
    props: {
        details: Object,
    }
}

</script>


<template>
    <div class="card">
        <div class="img">
            <img :src="details.thumb">
        </div>
        <p>
            {{ details.series }}
        </p>

    </div>
</template>


<style lang="scss" scoped>
.card {
    width: calc((100% / 12) * 2) - 1%;

    .img {
        height: 75%;

        img {
            width: 180px;
            height: 180px;
        }
    }

    p {
        color: white;
        text-transform: uppercase;
    }
}
</style>
