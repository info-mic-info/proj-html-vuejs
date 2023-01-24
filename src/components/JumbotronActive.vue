<script>
import { store } from "../store";

export default {
  data() {
    return {
      store,

      activeImage: 0,

      img_jumbotron: [
        {
          title: "SEM Campaigns Made Simple With Avada",
          paragraf:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates quaerat facere illum.",
          background: "1-hero-image.png",
        },
        {
          title: "Rank Your Local Business With SEO",
          paragraf: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",

          background: "agency-seo-desk-front-200x95.jpg",
        },
      ],
    };
  },
  methods: {
    setBackgroundHeader() {
      store.backgroundHeader = img_jumbotron[this.activeImage].background;
    },

    nextImage() {
      console.log("Avanti");
      this.activeImage++;
      if (this.activeImage > this.img_jumbotron.length - 1) {
        this.activeImage = 0;
      }
    },

    prevImage() {
      console.log("Indietro");
      this.activeImage--;
      if (this.activeImage < 0) {
        this.activeImage = this.img_jumbotron.length - 1;
      }
    },
  },
};
</script>


<!-- <img :src="img_jumbotron[activeImage].background"> -->

<template lang="">


    <!-- <img :src="`./src/assets/images/` + img_jumbotron[activeImage].background"> -->
  
  <div class="row prova">
    <div class="col-6">
      <div class="jumbotron py-5 pe-5">
        
        
<!-- ------------------------------------------ -->
<!-- TESTO ATTIVO -->
<ul>
<li><strong><h1>{{img_jumbotron[activeImage].title}}</h1></strong></li>
<li><p>{{img_jumbotron[activeImage].paragraf}} </p></li>
</ul>

<!-- ------------------------------------------ -->
        <button
          type="button"
          class="btn btn-warning radius me-3"
        >BUY AVADA NOW</button>
        <button
          type="button"
          class="btn btn-primary radius"
        >CONTACT US</button>
      </div>
      <div class="col-6"></div>
    </div>

    <div class="text-center">
      <button @click=" prevImage()">Indietro</button>
      <button @click=" nextImage()" >Avanti</button>
    </div>

  </div>
  <!-- IMMAGINE
_____________________________ -->
  <!-- <img :src="`/src/assets/images/` + img_jumbotron[0].background"> -->

  <!-- _______________________________ -->

</template>
<style lang="scss" scoped>
li {
  padding: 5px 0;
}

.prova {
  background-color: red;
}
</style>