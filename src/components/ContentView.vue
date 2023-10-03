<template>
  <div class="content-container">
    <div class="content-title">
      <h1>our creations</h1>
      <button>see all</button>
    </div>

    <div class="content-info">
      <div class="content-grid">
        <div class="content-item">
          <div class="content-img">
            <img
              class="desktop"
              src="../assets/images/desktop/image-deep-earth.jpg"
              alt=""
            />
            <img
              class="mobile"
              src="../assets/images/mobile/image-deep-earth.jpg"
              alt=""
            />
          </div>
          <div class="content-text">
            <h4>
              DEEP
              <br />
              EARTH
            </h4>
          </div>
        </div>
        <div class="content-item">
          <div class="content-img">
            <img
              class="desktop"
              src="../assets/images/desktop/image-night-arcade.jpg"
              alt=""
            />
            <img
              class="mobile"
              src="../assets/images/mobile/image-night-arcade.jpg"
              alt=""
            />
          </div>
          <div class="content-text">
            <h4>
              night
              <br />
              arcade
            </h4>
          </div>
        </div>
        <div class="content-item">
          <div class="content-img">
            <img
              class="desktop"
              src="../assets/images/desktop/image-soccer-team.jpg"
              alt=""
            />
            <img
              class="mobile"
              src="../assets/images/mobile/image-soccer-team.jpg"
              alt=""
            />
          </div>
          <div class="content-text">
            <h4>
              soccer
              <br />
              team vr
            </h4>
          </div>
        </div>
        <div class="content-item">
          <div class="content-img">
            <img
              class="desktop"
              src="../assets/images/desktop/image-grid.jpg"
              alt=""
            />
            <img
              class="mobile"
              src="../assets/images/mobile/image-grid.jpg"
              alt=""
            />
          </div>
          <div class="content-text">
            <h4>
              the
              <br />
              grid
            </h4>
          </div>
        </div>
        <div class="content-item">
          <div class="content-img">
            <img
              class="desktop"
              src="../assets/images/desktop/image-from-above.jpg"
              alt=""
            />
            <img
              class="mobile"
              src="../assets/images/mobile/image-from-above.jpg"
              alt=""
            />
          </div>
          <div class="content-text">
            <h4>
              from up
              <br />
              above vr
            </h4>
          </div>
        </div>
        <div class="content-item">
          <div class="content-img">
            <img
              class="desktop"
              src="../assets/images/desktop/image-pocket-borealis.jpg"
              alt=""
            />
            <img
              class="mobile"
              src="../assets/images/mobile/image-pocket-borealis.jpg"
              alt=""
            />
          </div>
          <div class="content-text">
            <h4>
              pocket
              <br />
              borealis
            </h4>
          </div>
        </div>
        <div class="content-item">
          <div class="content-img">
            <img
              class="desktop"
              src="../assets/images/desktop/image-curiosity.jpg"
              alt=""
            />
            <img
              class="mobile"
              src="../assets/images/mobile/image-curiosity.jpg"
              alt=""
            />
          </div>
          <div class="content-text">
            <h4>
              the
              <br />
              curiosity
            </h4>
          </div>
        </div>
        <div class="content-item">
          <div class="content-img">
            <img
              class="desktop"
              src="../assets/images/desktop/image-fisheye.jpg"
              alt=""
            />
            <img
              class="mobile"
              src="../assets/images/mobile/image-fisheye.jpg"
              alt=""
            />
          </div>
          <div class="content-text">
            <h4>
              make it
              <br />
              fisheye
            </h4>
          </div>
        </div>
      </div>

      <div class="content-action">
        <button>see all</button>
      </div>
    </div>
  </div>
</template>

<style scoped>
@import url("../assets/css/content.css");
</style>

<script>
import { reactive } from "vue";

export default {
  setup() {
    const state = reactive([]);

    return { state };
  },
};
</script>
