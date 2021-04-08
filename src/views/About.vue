<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
</template>

<script type="text/javascript" src="//code.jquery.com/jquery-1.11.0.min.js"></script>
<script type="text/javascript" src="//code.jquery.com/jquery-migrate-1.2.1.min.js"></script>
<script type="text/javascript" src="slick/slick.min.js"></script>

<script>
export default {
  mounted: function () {
    this.createSlick();
  },
  methods: {
    createSlick: function () {
      $(".multiple-items").slick({
        infinite: true,
        slidesToShow: 3,
        slidesToScroll: 3,
      });
    },
  },
};
</script>
