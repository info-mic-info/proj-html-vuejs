<script>
export default {};
</script>

<template lang="">
   <div class="container w-75">
    <div class="container w-50 text-center py-5">
    <h1><strong>Our Work</strong></h1>
    <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.</p>
    </div>
   </div>
   <div class="container w-75">
    <div class="row">
        <div class="col-4">
            <img src="../assets/images/case-study-gallery-3-1.jpg" alt="">
            <img class="hover" src="../assets/images/fss-demo-main-400x300.jpg" alt="">
        </div>
        <div class="col-4">
            <img src="../assets/images/case-study-gallery-2.jpg" alt="">
            <img class="hover" src="../assets/images/fss-demo-main-400x300.jpg" alt="">
        </div>
        <div class="col-4">
            <img src="../assets/images/case-study-gallery-1-1.jpg" alt="">
            <img class="hover" src="../assets/images/fss-demo-main-400x300.jpg" alt="">
        </div>
        <div class="col-4">
            <img src="../assets/images/case-study-gallery-4-1.jpg" alt="">
            <img class="hover" src="../assets/images/fss-demo-main-400x300.jpg" alt="">
        </div>
        <div class="col-4">
            <img src="../assets/images/case-study-gallery-5-1.jpg" alt="">
            <img class="hover" src="../assets/images/fss-demo-main-400x300.jpg" alt="">
        </div>
        <div class="col-4">
            <img src="../assets/images/case-study-gallery-6-1.jpg" alt="">
            <img class="hover" src="../assets/images/fss-demo-main-400x300.jpg" alt="">
        </div>
    </div>
    <div class="container text-center my-5">
    <button type="button" class="btn btn-warning radius">WIEW OUR WORK</button>
</div>
   </div>

</template> 

<style lang="scss" scoped>
.col-4 {
  padding: 0.5rem;
  position: relative;
  &:hover {
    .hover {
      opacity: 1;
      padding: 0.5rem;
    }
  }
}

.hover {
  padding: 0.5rem;
  position: absolute;
  top: 0;
  right: 0;
  left: 0;
  bottom: 0;
  object-fit: contain;
  opacity: 0;
  transition: opacity 0.4s;
}

img {
  width: 100%;
  object-fit: cover;
}
</style>