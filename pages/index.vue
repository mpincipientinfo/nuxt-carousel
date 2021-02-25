<template>
  <div class="carousel-wrapper">
    <div style="height:100px;width:500px">
      <client-only>
        <splide :options="options">
          <splide-slide>
            <img src="https://source.unsplash.com/random" /> </splide-slide
          ><splide-slide>
            <img src="https://source.unsplash.com/random" /> </splide-slide
          ><splide-slide>
            <img src="https://source.unsplash.com/random" /> </splide-slide
          ><splide-slide>
            <img src="https://source.unsplash.com/random" />
          </splide-slide>
        </splide>
      </client-only>
    </div>
  </div>
</template>

<script type="module">
export default {
  data() {
    return {
      options: {
        infinite: true,
        type: "loop",
        perPage: 3,
        dots: false,
        perMove: 1,
        pagination: false
      }
    };
  }
};
</script>
<style>
.splide__arrow--next {
  right: -8em !important;
}
.splide__arrow--prev {
  left: -8em !important;
}
.splide__arrow {
  box-sizing: border-box !important;
  font-weight: 30px;
  height: 50px;
  width: 50px;
  border-radius: 5px;
  background-color: #555;
}
.carousel-wrapper {
  margin-left: 155px;
}
</style>
