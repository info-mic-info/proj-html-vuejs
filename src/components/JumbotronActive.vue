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
  
  <div class="row w-50">
    <div class="col">
      <div class="jumbotron py-5 pe-5 margintitle">
        
        
<!-- ------------------------------------------ -->
<!-- TESTO ATTIVO -->
<h1><strong>{{img_jumbotron[activeImage].title}}</strong></h1>
<p>{{img_jumbotron[activeImage].paragraf}} </p>


<!-- ------------------------------------------ -->
</div>
<div class="container">
<button
type="button"
class="btn btn-warning radius me-3"
>BUY AVADA NOW</button>
<button
type="button"
class="btn btn-primary radius"
        >CONTACT US</button>
      </div>



    
    </div>
    
    <i @click=" prevImage()" class="fa-solid fa-chevron-left arrow left"></i>
    <i @click=" nextImage()" class="fa-solid fa-chevron-right arrow right"></i>


  </div>
  <!-- IMMAGINE
_____________________________ -->
  <!-- <img :src="`/src/assets/images/` + img_jumbotron[0].background"> -->

  <!-- _______________________________ -->

</template>
<style lang="scss" scoped>
.jumbotron {
  height: 250px;
}
.row {
  color: white;
}
.arrow {
  width: 40px;
  height: 50px;
  background-color: black;
  color: white;
  opacity: 0.5;
  display: flex;
  justify-content: center;
  align-items: center;
}

.right {
  position: absolute;
  right: 5px;
  top: 30%;
}

.left {
  position: absolute;
  left: 5px;
  top: 30%;
}
li {
  padding: 5px 0;
}

.row {
  height: 600px;
}
.margintitle {
  margin-top: 100px;
}
</style>