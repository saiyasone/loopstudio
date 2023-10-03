<template>
  <header>
    <nav>
      <div class="nav-brand">
        <div class="nav-mobile"></div>
        <a href="#">loopstudios</a>
      </div>

      <ul>
        <template v-for="(item, index) in state.navBar" :key="index">
          <li>
            <a href="#">
              {{ item }}
            </a>
          </li>
        </template>
        <div @click="setToggle()" class="nav-mobile">
          <img src="../assets/images/icon-hamburger.svg" alt="" />
        </div>
      </ul>
    </nav>
  </header>

  <!-- <template v-if="state.toggle"> -->
  <SideBar
    :toggle="state.toggle"
    :navBars="state.navBar"
    @close="setToggle()"
  ></SideBar>
  <!-- </template> -->
</template>

<script>
import { reactive, onMounted } from "vue";
import SideBar from "./SideBarView.vue";
export default {
  props: ["navItems"],
  components: {
    SideBar,
  },
  setup(props) {
    const state = reactive({
      toggle: false,
      navBar: props.navItems,
    });

    function setToggle() {
      state.toggle = !state.toggle;
    }

    onMounted(() => {
      window.addEventListener("resize", (e) => {
        let width = e.target.innerWidth;
        if (width <= 900) {
          state.toggle = false;
        }
      });
    });

    return {
      state,

      setToggle,
    };
  },
};
</script>

<style scoped>
@import url("../assets/css/header.css");
</style>
