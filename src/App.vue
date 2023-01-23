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
    <AppHeader/>
  </div>

<AppMain/>

<AppFooter/>
  
  
</template>


<style lang="scss">
@use "./styles/generals.scss" as *;

.background {
  background-image: url("./assets/images/1-hero-image.png");
  background-size: cover;
  color: white;
  height: 1000px;
}
</style>