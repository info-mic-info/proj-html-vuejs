<script>
import NavBar from "./NavBar.vue";
import Jumbotron from "./Jumbotron.vue";
export default {
  components: {
    NavBar,
    Jumbotron,
  },
  data() {
    return {
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
  <header class="d-flex justify-content-between ">

    <img
      src="../assets/images/logo_seo_w_2x.png"
      alt=""
    >

    <div class="Container-fluid d-flex ">
      <ul class="d-flex margin-auto">
        <NavBar
          v-for="(item, index) in items"
          :key="index"
          :itemsNav="item"
        />
      </ul>
      <button type="button" class="btn btn-warning">CONTACT US</button>
    </div>
  </header>
  <Jumbotron />

</template>


<style lang="scss" scoped>
.margin-auto {
  margin: auto 0;
}
</style>