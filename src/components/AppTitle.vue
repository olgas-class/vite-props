<script>
export default {
    name: "AppTitle",
    props: ["titleText", "subtitleText"]
}
</script>

<template>
    <div class="title">
        <h2>{{ titleText }}</h2>
        <p>{{ subtitleText }}</p>
    </div>

</template>

<style scoped>
.title {
    text-align: center;
    margin-bottom: 1rem;
}
</style>