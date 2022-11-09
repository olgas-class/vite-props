<script>
export default {
    name: "AppBanner",
    props: {
        img: String,
        title: String
    },
    methods: {
        getImageUrl(url) {
            return new URL(url, import.meta.url).href;
        }
    }
}
</script>

<template>
    <div class="banner">
        <img :src="getImageUrl(`../assets/img/${img}`)" alt="">
        <h2>{{ title }}</h2>
    </div>

</template>

<style scoped>
.banner {
    position: relative;
    width: 100%;
    height: 400px;
}

.banner img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.banner h2 {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
</style>