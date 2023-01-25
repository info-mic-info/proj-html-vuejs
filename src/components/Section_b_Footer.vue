<script>
export default {};
</script>


<template lang="">
<div class="col-12">
    <img class="img-fluid w-100" src="../assets/images/CTA-seo-1.jpg" alt="">


    <div class="container w-25 py-2">
        <ul class="text-center">
            <li><h2><strong>Start Your Free Consultation</strong></h2></li>
            <li><p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.</p></li>
            <li><button type="button" class="btn btn-warning radius">CONTACT US NOW</button></li>
    </ul>
  
</div>


</div>


</template>


<style lang="scss" scoped>
img {
  filter: brightness(30%);
}

li {
  padding: 10px 0;
}

.btn {
  background-color: orange;
}

.col-12 {
  position: relative;
  .container {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: white;
  }
}
</style>