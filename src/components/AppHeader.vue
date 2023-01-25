<script>
import { store } from "../store";
import NavBar from "./NavBar.vue";
import JumbotronActive from "./JumbotronActive.vue";
export default {
  components: {
    NavBar,
    JumbotronActive,
  },
  data() {
    return {
      store,
      items: [
        {
          label: "Home",
          url: "#",
          active: false,
        },
        {
          label: "Who We Are",
          url: "#",
          active: true,
        },
        {
          label: "Who We Are",
          url: "#",
          active: false,
        },
        {
          label: "Who We Work",
          url: "#",
          active: false,
        },
        {
          label: "Careers",
          url: "#",
          active: false,
        },
        {
          label: "News",
          url: "#",
          active: false,
        },
      ],
    };
  },
};
</script>


<template lang="" >
    <!-- <header> -->
        <header style=" background-size: cover; background-image: url('/1-hero-image.png')">
          <!-- <img :src="`./src/assets/images/` + store.backgroundHeader"> -->
        <div class="container w-75 pt-4 ">

          <div class="flex">
        <div class="logo d-flex">  
    <img
      src="../assets/images/logo_seo_w_2x.png"
      alt=""
    >
      <ul class="d-flex margin-auto">
        <NavBar
          v-for="(item, index) in items"
          :key="index"
          :itemsNav="item"
        />
      </ul>
    </div>
<div class="button">
      <button type="button" class="btn btn-warning radius">CONTACT US</button>
    </div>
  </div>
    </div>
  

<div class="container w-75">
  <JumbotronActive/> 

</div>
  </header>




</template>


<style lang="scss" scoped>
header {
  color: white;
}
.flex {
  display: flex;
  justify-content: space-between;
}

.margin-auto {
  margin: auto 0;
}

img {
  width: 15%;
}
</style>