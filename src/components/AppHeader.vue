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
    <header>
        <!-- <header :style="{background-image: url(store.backgroundHeader)}"> -->
          <img :src="`./src/assets/images/` + store.backgroundHeader">
        <div class="container d-flex w-75">
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
   
      <button type="button" class="btn btn-warning radius">CONTACT US</button>
    </div>
  

<div class="container w-75">
  <JumbotronActive/> 


  
</div>

  </header>




</template>


<style lang="scss" scoped>
.margin-auto {
  margin: auto 0;
}

img {
  width: 15%;
}
</style>