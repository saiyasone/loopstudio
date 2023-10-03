<template>
  <div class="home-container">
    <div class="home-info">
      <div class="home-text">
        <h2>immersive experiances that deliver</h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  setup() {},
};
</script>

<style scoped>
.home-container {
  max-width: 1200px;
  padding: 0 25px;
  margin: 0 auto;
}

.home-container .home-info {
  max-width: 550px;
  padding-top: 6rem;
}

.home-info .home-text {
  position: relative;
  border: 3px solid #fff;
  padding: 2.5rem;
}

.home-text h2 {
  font-size: 4rem;
  color: #fff;
  text-transform: uppercase;
  font-weight: 300;
  line-height: 1;
}

@media (max-width: 992px) {
  .home-container .home-info {
    margin: 0 auto;
  }
}
@media (max-width: 650px) {
  .home-info .home-text {
    padding: 2rem;
  }
  .home-text h2 {
    font-size: 3.5rem;
  }
}

@media (max-width: 550px) {
  .home-text h2 {
    font-size: 2.5rem;
  }
}
</style>
