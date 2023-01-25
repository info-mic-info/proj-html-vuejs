<script>
export default {
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


<template lang="">
<div class="container text-center w-75 py-5">
  <div class="container my-5">
    <img src="../assets/images/logo_seo_2x.png" alt="">
  </div>

<div class="container">
  <ul class="d-flex justify-content-center">
    <li v-for="(item, index) in items" :key="index" class="items">{{item.label}}</li>
  </ul>
</div>


    <div class="container copyright">
    <ul class="d-flex justify-content-center">
        <li>© Copyright 2017</li>
        <li>|</li>
        <li>Avada Theme <a href="">by ThemeFusion</a></li>
        <li>|</li>
        <li>All Rights Reserved</li>
        <li>|</li>
        <li>Powered by <a href="">WordPress</a></li>
    </ul>
  </div>

    <div class="container">
    <ul class="d-flex justify-content-center">
        <li><i class="fa-brands fa-facebook-f"></i></li>
        <li><i class="fa-brands fa-instagram"></i></li>
        <li><i class="fa-brands fa-twitter"></i></li>
        <li><i class="fa-brands fa-youtube"></i></li>
        <li><i class="fa-brands fa-linkedin-in"></i></li>
    </ul>
  </div>
</div>







</template>


<style lang="scss" scoped>
img {
  width: 250px;
}
li {
  margin: 0 12px;
}
.copyright {
  li {
    margin: 0 5px;
  }
}

i {
  font-size: 20px;
  color: rgba(27, 26, 26, 0.701);
}

a {
  color: orange;
  text-decoration: none;
}
</style>