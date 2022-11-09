<script>
export default {
    name: "HeroCard",
    props: {
        heroName: String,
        imgSrc: String
    }
}
</script>

<template>
    <h2>{{ heroName }}</h2>
    <img :src="imgSrc" :alt="heroName">
</template>

<style scoped>

</style>