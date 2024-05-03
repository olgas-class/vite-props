<script>
import SectionBanner from "./components/SectionBanner.vue";
import SectionTitle from "./components/SectionTitle.vue";
export default {
  components: {
    SectionTitle,
    SectionBanner,
  },
  data() {
    return {
      bannersArray: [
        {
          color: "lightblue",
          image:
            "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.G37tgeQqSNt7v2oPfj9ltQHaE7%26pid%3DApi&f=1&ipt=64c6c979c6e1446b1b100459f59a4032dddbba516ed6e1058877b57715ecac0b&ipo=images",
          title: "First banner",
          text: "Thi is my first banner",
        },
        {
          color: "lightgreen",
          image:
            "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.ErAiMih0ltX9nxzgEbfN0gHaEp%26pid%3DApi&f=1&ipt=fb0b8de2d956884401fd84357fb0b8bc64f5e6f162b3a0a899ef89d0d8fcce3e&ipo=images",
          title: "Second banner",
          text: "Thi is my second banner",
        },
        {
          color: "orange",
          image:
            "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.KY__xOOKjP59qHzyduyntgHaE8%26pid%3DApi&f=1&ipt=de129d85a7d320c8ae0575acac78b59882ae1c4292037a8834a390d3918e4f23&ipo=images",
          title: "Third banner",
          text: "Thi is my Third banner",
        },
      ],
    };
  },
};
</script>

<template>
  <main>
    <!-- Banners section -->
    <section>
      <SectionBanner
        v-for="banner in bannersArray"
        :bannerTitle="banner.title"
        :bannerText="banner.text"
        :bannerColor="banner.color"
        :bannerImage="banner.image"
      />
    </section>
    <!-- /Banners section -->

    <!-- About us section -->
    <section>
      <SectionTitle title="Chi siamo" subtitle="Siamo una squadra fortissima" />
      <div>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsum ab quos
        doloribus, corporis, consequatur quisquam et ipsam numquam ea, dolores
        cum pariatur quam. Sed rem aperiam, mollitia ea facilis sint? Ex quaerat
        facilis blanditiis repudiandae mollitia autem non quae commodi aperiam
        officiis quasi nemo, possimus similique quisquam impedit veritatis
        expedita? Iusto quo dolores necessitatibus quas veniam perspiciatis
        eaque harum enim? Similique ipsa voluptatem voluptas eum ipsam expedita,
        illum eveniet quasi numquam nihil inventore provident culpa harum
        blanditiis debitis natus mollitia ullam dignissimos aliquam placeat est
        voluptate distinctio cupiditate. Praesentium, recusandae.
      </div>
    </section>
    <!-- /About us section -->

    <!-- Our services section -->
    <section>
      <SectionTitle
        title="Nostri servizi"
        subtitle="Tutto quello di cui hai bisogno nel web"
      />

      <div>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur
        libero assumenda consequuntur ipsum dolor, vero doloribus eaque nihil
        labore. Accusantium doloribus odio quos ad ullam. Molestiae, porro
        repudiandae? Officia, provident? Qui, ab nulla tempore veritatis quaerat
        ipsa voluptate autem id alias ea expedita impedit, suscipit numquam
        recusandae necessitatibus. Iusto perferendis ad dicta. Nihil inventore
        quasi delectus modi minima non quas. Reiciendis sint natus doloremque
        repellendus cupiditate et soluta, accusamus maxime atque in qui ipsa
        animi quae fuga delectus. Consequuntur hic totam consectetur dolor,
        voluptatum non! Laboriosam voluptate perspiciatis ad tempore.
        Voluptatibus magni delectus culpa maiores distinctio explicabo similique
        blanditiis repellendus consequuntur, nihil ad incidunt fugiat beatae
        tempore error, excepturi sed sequi aspernatur? Odio molestias, impedit
        ex iusto fugit maiores tenetur.
      </div>
    </section>
    <!-- /Our services section -->
  </main>
</template>

<style lang="scss"></style>
