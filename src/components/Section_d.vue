        <script>
export default {};
</script>

<template lang="">
  <section class="background_d">
    <div class="container w-75 py-5">
    <div class="container w-50 text-center">
    <h1><strong>Our Plans</strong></h1>
    <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.</p>
  </div>

  <div class="container py-5">
    <div class="row d-flex justify-content-between">
      <div class="col text-center">
        <h4><strong>Standard</strong></h4>
        <div class="price d-flex justify-content-center">
          <div><h6>$</h6></div>
          <div><h1>19</h1></div>
          <div><h6>99</h6> <p>Monthtly</p></div>
        </div>
        <div class="info">
        <p>5 Projects</p>
        <p>5 GB Storage</p>
        <p>Unlimited Users</p>
      </div>
        <button type="button" class="btn btn-outline-secondary radius my-4">START TODAY</button>
      </div>
      <div class="col text-center">
        <h4><strong>Premium</strong></h4>
        <div class="price d-flex justify-content-center">
          <div><h6>$</h6></div>
          <div><h1>29</h1></div>
          <div><h6>99</h6> <p>Monthtly</p></div>
        </div>
        <div class="info">
        <p>10 Projects</p>
        <p>15 GB Storage</p>
        <p>Unlimited Users</p>
      </div>
        <button type="button" class="btn btn-outline-secondary radius my-4">START TODAY</button>
      </div>
      <div class="col text-center">
        <h4><strong>Professional</strong></h4>
        <div class="price d-flex justify-content-center">
          <div><h6>$</h6></div>
          <div><h1>39</h1></div>
          <div><h6>99</h6> <p>Monthtly</p></div>
        </div>
        <div class="info">
        <p>15 Projects</p>
        <p>30 GB Storage</p>
        <p>Unlimited Users</p>
      </div>
        <button type="button" class="btn btn-outline-secondary radius my-4">START TODAY</button>
      </div>
      
      <div class="col text-center">
        <h4><strong>Extreme</strong></h4>
        <div class="price d-flex justify-content-center">
          <div><h6>$</h6></div>
          <div><h1>59</h1></div>
          <div><h6>99</h6> <p>Monthtly</p></div>
        </div>
        <div class="info">
        <p>Unlimited Projects</p>
        <p>Unlimited Storage</p>
        <p>Unlimited Users</p>
      </div>
        <button type="button" class="btn btn-outline-secondary radius my-4">START TODAY</button>
      </div>

   
    </div>
  </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.background_d {
  background-image: url("../assets/images/background1.jpg");
  color: white;
}

.btn {
  color: black;

  &:hover {
    background-color: orange;
  }
}

.info {
  p {
    padding: 10px 0;
  }
}

h4 {
  padding: 20px 0;
  color: rgb(96, 122, 254);
}

.col {
  background-color: white;
  color: black;
  padding: 10px;
  margin: 10px;
}

.price {
  padding: 10px 0;
  p {
    font-size: 8px;
    font-weight: bold;
  }
  h1,
  h6 {
    font-weight: bold;
    text-align: left;
    color: rgb(96, 122, 254);
  }
}
</style>