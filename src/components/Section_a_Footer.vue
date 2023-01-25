<script>
export default {
  data() {
    return {
      activeImage: 0,

      img_circle: [
        {
          image: "testimonials-2.jpg",
          paragraf:
            "Ability proceeds from a fusion of skill, Knowledge, understanding and imagination, consolidated by experience.",
          nameavatar: "Luis Desalvo",
          work: "CREO TECH",
        },
        {
          image: "testimonials-1.jpg",
          paragraf:
            "Beauty is when you can appreciate yourself. When you love yourself, that’s when you’re most beautiful.",
          nameavatar: "Shelia McCourtney",
          work: "ARCHITECT",
        },
      ],
    };
  },
  methods: {
    nextImage() {
      console.log("Avanti");
      this.activeImage++;
      if (this.activeImage > this.img_circle.length - 1) {
        this.activeImage = 0;
      }
    },

    prevImage() {
      console.log("Indietro");
      this.activeImage--;
      if (this.activeImage < 0) {
        this.activeImage = this.img_circle.length - 1;
      }
    },
  },
};
</script>


<template lang="">
    <div class="container w-75 text-center py-5">
        <ul>
            <li> <h2><strong>What Our Client Say</strong></h2></li>
            <li> <img :src="`/src/assets/images/`+ img_circle[this.activeImage].image"></li>
            <li><p><i>{{img_circle[this.activeImage].paragraf}}</i></p></li>
            <li><p><strong>{{img_circle[this.activeImage].nameavatar}}</strong>, {{img_circle[this.activeImage].work}} </p></li>
        </ul>
        <div class="container pb-5">
       
            <i  v-for="(item, index) in img_circle" 
                    :class="(activeImage === index) ? `fa-solid fa-circle` : ``" class="fa-regular fa-circle me-1" @click=" nextImage()" ></i>
            <!-- <i class="fa-regular fa-circle ms-1" @click=" prevImage()"></i> -->
        </div>
        <hr>
       
       <div class="container py-3">
        <div class="row d-flex justify-content-center">
            <div class="col-3">
                <img src="../assets/images/clients_partner_5-200x202.png" alt="">
            </div>

            <div class="col-3">
                <img src="../assets/images/clients_partner_6-200x202.png" alt="">
            </div>

            <div class="col-3">
                <img src="../assets/images/clients_partner_1-200x202.png" alt="">
            </div>

            <div class="col-3">
                <img src="../assets/images/clients_partner_2-200x202.png" alt="">
            </div>

        </div>
       </div>
    
     
    </div>
</template>


<style lang="scss" scoped>
ul img {
  border-radius: 100%;
}

li {
  margin: 20px 0;
}

.col-3 img {
  width: 80px;
}

.active {
  color: black;
}
</style>