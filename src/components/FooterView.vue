<template>
  <div class="footer-container">
    <div class="footer-top-container">
      <div class="footer-top">
        <div class="footer-brand">
          <a href="#">loopstudios</a>
        </div>
        <div class="footer-social">
          <a href="#" class="social-icon">
            <img src="../assets/images/icon-facebook.svg" alt="" />
          </a>
          <a href="#" class="social-icon">
            <img src="../assets/images/icon-twitter.svg" alt="" />
          </a>
          <a href="#" class="social-icon">
            <img src="../assets/images/icon-pinterest.svg" alt="" />
          </a>
          <a href="#" class="social-icon">
            <img src="../assets/images/icon-instagram.svg" alt="" />
          </a>
        </div>
      </div>
      <div class="footer-center">
        <ul>
          <li v-for="nav in navItems" :key="nav">
            <a href="#">
              {{ nav }}
            </a>
          </li>
        </ul>

        <div class="license">
          <p>© {{ today }} Loopstudio. All rights reserved.</p>
        </div>
      </div>
    </div>

    <div class="footer-down"></div>
  </div>
</template>

<script>
export default {
  props: ["navItems"],
  data() {
    return {
      today: new Date().getFullYear(),
    };
  },
};
</script>

<style scoped>
@import url("../assets/css/footer.css");
</style>
