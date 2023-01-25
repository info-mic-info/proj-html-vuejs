<script>
export default {};
</script>

<template>
  <section class="background_e">
    <div class="container w-75 py-5">
      <div class="container w-50 text-center py-5">
        <h1 class="mb-3"><strong>Latest News</strong></h1>
        <p>ed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.</p>
      </div>
      <div class="container text-center">
        <div class="row">
          <div class="col-4">
            <div class="image">
              <img
                src="../assets/images/related-service-2-700x441.jpg"
                alt=""
              >
            </div>
            <h6 class="pt-4"><strong>Why You Need A SEO Agency Now</strong></h6>
            <p class="miniature">November 1st, 2017</p>
            <p>ALorem ipsum dolor sit amet, consectetur adipiscing elit. In et scelerisque sem. Nunc molestie neque augue, at gravida mi blandit</p>
          </div>

          <div class="col-4">
            <div class="image">
              <img
                src="../assets/images/related-service-4-700x441.jpg"
                alt=""
              >
            </div>
            <h6 class="pt-4"><strong>SEO Tips For Your Startup</strong></h6>
            <p class="miniature">November 1st, 2017</p>
            <p>ALorem ipsum dolor sit amet, consectetur adipiscing elit. In et scelerisque sem. Nunc molestie neque augue, at gravida mi blandit</p>
          </div>

          <div class="col-4">
            <div class="image">
              <img
                src="../assets/images/blog-post-6-700x441.jpg"
                alt=""
              >
            </div>
            <h6 class="pt-4"><strong>Image Optimization For Your Site</strong></h6>
            <p class="miniature">November 1st, 2017</p>
            <p>ALorem ipsum dolor sit amet, consectetur adipiscing elit. In et scelerisque sem. Nunc molestie neque augue, at gravida mi blandit</p>
          </div>

        </div>
      </div>
      <div class="container text-center py-5">
        <button
          type="button"
          class="btn btn-warning radius"
        >GO TO NEWS</button>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.background_e {
  background-color: #f8f8f8;
}

.miniature {
  font-size: 12px;
}

.image {
  overflow: hidden;
}

img {
  width: 100%;
  transition: transform 0.6s;
  object-fit: cover;
}

.image:hover img {
  transform: scale(1.1);
}

h6 {
  color: orange;
}
</style>