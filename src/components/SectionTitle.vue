<script>
export default {
  props: {
    title: String,
    subtitle: String,
  },
};
</script>

<template>
  <div class="title-wrapper">
    <h2>{{ title }}</h2>
    <p>{{ subtitle }}</p>
  </div>
</template>

<style scoped lang="scss">
.title-wrapper {
  text-align: center;
  margin: 1rem 0;

  h2 {
    padding: 0.5rem 1rem;
    font-size: 2.5rem;
  }

  p {
    font-style: italic;
  }
}
</style>
