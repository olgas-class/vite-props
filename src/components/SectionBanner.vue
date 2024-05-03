<script>
export default {
  props: {
    bannerColor: String,
    bannerImage: String,
    bannerTitle: String,
    bannerText: String,
  },
};
</script>

<template>
  <div
    class="banner"
    :style="{
      'background-color': bannerColor,
      'background-image': `url(${bannerImage})`,
    }"
  >
    <div class="banner-inner">
      <h3>{{ bannerTitle }}</h3>
      <p>{{ bannerText }}</p>
    </div>
  </div>

  <!-- <img :src="bannerImage" alt="" /> -->
</template>

<style scoped lang="scss">
.banner {
  padding: 5rem 0;
  border: 2px solid black;
  background-size: cover;
  background-position: center;

  .banner-inner {
    width: 70%;
    margin: 0 auto;
    text-align: center;

    h3 {
      font-size: 2rem;
    }
  }
}
</style>
