<template>
  <div>
    <VueSlickCarousel v-bind="settings" class="carousel">
      <div>
        <img
          v-bind:src="'https://resizing.flixster.com/gFjkV0hWWFFhN2qrf_P_j-1-KSQ=/506x652/v2/https://flxt.tmsimg.com/v9/AllPhotos/258/258_v9_bb.jpg'"
          class="cage-pic"
        />
      </div>
      <div>
        <img
          v-bind:src="'https://upload.wikimedia.org/wikipedia/commons/f/f3/Nicolas_Cage_-_66%C3%A8me_Festival_de_Venise_%28Mostra%29.jpg'"
          class="cage-pic"
        />
      </div>
      <div>
        <img v-bind:src="'https://i.redd.it/e0wni1by9zm31.jpg'" class="cage-pic" />
      </div>
      <div>
        <img
          v-bind:src="'https://img.cinemablend.com/filter:scale/quill/2/5/7/3/b/2/2573b2c3b5ebe45b398fcb9c10538e6c10a5c60b.jpg?mw=600'"
          class="cage-pic"
        />
      </div>
      <div>
        <img v-bind:src="'https://pbs.twimg.com/profile_images/954732522952421376/QS3bZT23.jpg'" class="cage-pic" />
      </div>
      <div>
        <img v-bind:src="'https://pbs.twimg.com/media/EJk1ypoVUAAPNTR.jpg'" class="cage-pic" />
      </div>
    </VueSlickCarousel>
  </div>
</template>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// optional style for arrows & dots
import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";

export default {
  name: "MyComponent",
  components: { VueSlickCarousel },
  data: function () {
    return {
      settings: {
        dots: true,
        infinite: true,
        initialSlide: 0,
        speed: 500,
        slidesToShow: 3,
        slidesToScroll: 1,
        swipeToSlide: true,
      },
    };
  },
};
</script>

<style>
.cage-pic {
  height: 250px;
  width: 200px;
  margin-left: auto;
  margin-right: auto;
}

.carousel {
  height: 250px;
  width: 750px;
  margin-left: auto;
  margin-right: auto;
}
</style>
