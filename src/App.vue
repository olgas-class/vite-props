<script>
import AppTitle from './components/AppTitle.vue';
import AppBanner from './components/AppBanner.vue';
import HeroCard from './components/HeroCard.vue';
export default {
  components: {
    AppTitle,
    AppBanner,
    HeroCard
  },
  data() {
    return {
      banners: [
        {
          bannerImg: 'fondo-pag-speciali.jpg',
          bannerTitle: 'Primo titolo'
        },
        {
          bannerImg: 'footer-montagne-bottom.jpg',
          bannerTitle: 'Secondo titolo'
        },
      ],
      superheros: [
        {
          img: "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse3.mm.bing.net%2Fth%3Fid%3DOIP.CVog2TrZJv0P3ZhmOAVC2gHaJl%26pid%3DApi&f=1&ipt=0ad039f1a1f813ff3991ffb1966b4355e56e5cc0f2eac064dd5c899c818b16e7&ipo=images",
          name: "Superman"
        },
        {
          img: "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse3.mm.bing.net%2Fth%3Fid%3DOIP.wEMrHlwA6p7JDFiVtAtgNAHaHa%26pid%3DApi&f=1&ipt=8ea67291556184109d82e3105adbd6f3cb8a5bb698b50c5bd353e21d20f6beaf&ipo=images",
          name: "Hulk"
        },
        {
          img: "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.TCPVFnrqmggPc2RG8bhHAQHaEK%26pid%3DApi&f=1&ipt=7e80d5b506b5152f6add48d53f9c9a3124a8460f61194180a3c2a0f607087d6f&ipo=images",
          name: "Spiderman"
        }
      ]
    }
  }
}
</script>

<template>
  <!-- <section>
    <AppTitle :titleText="'Nostri servizi'" :subtitleText="'le nostre migliori offerte'" />
  </section>

  <AppBanner :img="'fondo-pag-speciali.jpg'" />

  <section>
    <AppTitle :titleText="'Nostro team'" :subtitleText="'Insieme si vince'" />
  </section>

  <AppBanner :img="'footer-montagne-bottom.jpg'" /> -->
  <!-- 
  <AppBanner v-for="(item, index) in banners" :key="index" :img="item.bannerImg" :title="item.bannerTitle" /> -->

  <section>
    <HeroCard v-for="(hero, index) in superheros" :key="index" :heroName="hero.name" :imgSrc="hero.img" />
  </section>

</template>

<style>

</style>