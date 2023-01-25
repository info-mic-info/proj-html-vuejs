        <script>
export default {};
</script>


<template lang="">
    <section class="background-blue">

        
        <div class="container w-75 paddingplus ">
            <div class="container w-50 text-center">
        <h1 class="mb-4"><strong>See our Top Notch Services</strong></h1>
        <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.</p>
        </div>

        </div>
        <div class="container w-75 paddingcard">

    <div class="mycard text-center">
        <div class="row d-flex justify-content-between">


  <div class="col">
  <ul>
    <div class="orange">
      <div class="container-fluid child bounce">
   <li> <i class="fa-brands fa-google"></i></li>
  </div>
    <li><h4><strong>Google SEO</strong></h4></li>
  
  </div>
    <li><p>Vestibulum in lacinia metus. Suspendisse in enim ipsum. Nulla facilisi. Donec ante turpis, dictum sed magna et dapibus faucibus odio.</p></li>
    <li><h6>Let's work together></h6></li>
  </ul>
</div>



<div class="col">
  <ul>
    <div class="orange">
      <div class="container-fluid child bounce">
  <li> <i class="fa-solid fa-gear"></i></li> 
</div>
  <li> <h4><strong>Brand Strategy</strong></h4></li> 
</div>
   <li><p>Vestibulum in lacinia metus. Suspendisse in enim ipsum. Nulla facilisi. Donec ante turpis, dictum sed magna et dapibus faucibus odio.</p></li> 
   <li> <h6>Let's work together></h6></li>
  </ul>
</div> 

<div class="col">
  <ul>
    <div class="orange">
      <div class="container-fluid child bounce">
    <li><i class="fa-solid fa-building"></i></li>
  </div>
    <li><h4><strong>Local SEO</strong></h4></li>
  </div>
    <li><p>Vestibulum in lacinia metus. Suspendisse in enim ipsum. Nulla facilisi. Donec ante turpis, dictum sed magna et dapibus faucibus odio.</p></li>
    <li><h6>Let's work together></h6></li>
  </ul>
</div>

<div class="col">
  <ul>
    <div class="orange">
      <div class="container-fluid child bounce">
   <li> <i class="fa-solid fa-chart-column"></i></li>
  </div>
    <li><h4><strong>SEO Analysis</strong></h4></li>
  </div>
    <li><p>Vestibulum in lacinia metus. Suspendisse in enim ipsum. Nulla facilisi. Donec ante turpis, dictum sed magna et dapibus faucibus odio.</p></li>
    <li><h6>Let's work together></h6></li>
  </ul>
</div>
        </div>
    </div>
</div>
</section>
</template>


<style lang="scss" scoped>
.orange:hover {
  h4 {
    color: orange;
  }
  .bounce {
    animation-name: bounce;
    animation-timing-function: ease;
  }
  @keyframes bounce {
    0% {
      transform: translateY(0);
    }
    25% {
      transform: translateY(-10px);
    }
    50% {
      transform: translateY(-15px);
    }
    75% {
      transform: translateY(-10px);
    }
    100% {
      transform: translateY(0);
    }
  }
}

.child {
  animation-duration: 0.2s;
  transform-origin: bottom;
}

.background-blue {
  background-image: url("../assets/images/pattern_background.png");
  background-color: #051745;
  color: white;
}

.paddingplus {
  padding: 50px 0;
}
.paddingcard {
  padding-bottom: 130px;
  padding-top: 50px;
}
.col {
  background-color: rgb(0, 16, 97);
  padding: 40px;
  margin: 6px;
}

li {
  padding: 10px 0;
}

i {
  color: orange;
  font-size: 40px;
}

h4:hover {
  color: orange;
}

h6 {
  color: orange;
}
</style>