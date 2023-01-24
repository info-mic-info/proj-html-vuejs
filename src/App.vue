    <script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  },
};
</script>


<template lang="">
  <div class="background">
    <div class="container w-75">
    <AppHeader/>
  </div>
  </div>

<AppMain/>

<AppFooter/>
  
  
</template>


<style lang="scss">
@use "./styles/generals.scss" as *;

.background {
  background-image: url("./assets/images/1-hero-image.png");
  background-size: cover;
  width: 100%;
  background-repeat: no-repeat;
  color: white;
  height: 500px;
}
</style>