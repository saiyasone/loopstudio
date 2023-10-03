<template>
  <div class="home-wrapper">
    <!-- ======== Header ========= -->
    <Header :navItems="navItems" />

    <Home />
  </div>

  <main>
    <div class="container">
      <!-- ======== Leader ========= -->
      <section class="section-leader">
        <Lead />
      </section>

      <!-- ======== Content ========= -->
      <section class="section-content">
        <Content />
      </section>
    </div>
  </main>

  <div class="footer">
    <Footer :navItems="navItems" />
  </div>
</template>

<script>
import Header from "./components/HeaderView.vue";
import Home from "./components/HomeView.vue";
import Lead from "./components/LeaderView.vue";
import Content from "./components/ContentView.vue";
import Footer from "./components/FooterView.vue";
export default {
  name: "App",
  components: {
    Lead,
    Home,
    Header,
    Footer,
    Content,
  },

  data() {
    return {
      navItems: ["about", "careers", "events", "products", "support"],
    };
  },
};
</script>

<style>
@import url("./assets/css/style.css");
</style>
