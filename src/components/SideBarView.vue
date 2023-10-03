<template>
  <aside :class="{ toggle: toggle }">
    <div class="side-container">
      <div class="side-header">
        <a href="#">loopstudios</a>
        <div @click="onClose()" class="close">
          <img src="../assets/images/icon-close.svg" alt="" />
        </div>
      </div>
      <div class="side-nav">
        <ul>
          <li v-for="(item, index) in navBars" :key="index">
            <a href="#">
              {{ item }}
            </a>
          </li>
        </ul>
      </div>
    </div>
  </aside>
</template>

<script>
export default {
  props: ["navBars", "toggle"],
  emits: ["close"],

  methods: {
    onClose() {
      this.$emit("close");
    },
  },
};
</script>

<style scoped>
@import url("../assets/css/sidebar.css");
</style>
