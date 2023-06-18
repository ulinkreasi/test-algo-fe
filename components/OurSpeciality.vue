<template>
  <section style="background-color: #509fdd" class="p-5">
    <div class="d-flex flex-column p-5" style="background-color: #fff">
      <div class="row justify-content-center">
        <h1 style="color: #029fe4">{{ title }}</h1>
      </div>
      <div class="row justify-content-center">
        <p class="ml-4 align-items-end" style="color: #303030">
          {{ description }}
        </p>
      </div>
      <b-row class="justify-content-center">
        <div style="max-width: 700px">
          <b-carousel
            id="carousel-1"
            v-model="slide"
            :interval="0"
            controls
            indicators
            background="#white"
            img-width="700"
            img-height="480"
            style="text-shadow: 1px 1px 2px #333"
          >
            <!-- Slides with img slot -->
            <!-- Note the classes .d-block and .img-fluid to prevent browser default image alignment -->
            <b-carousel-slide>
              <template #img>
                <img
                  class="d-block center-block"
                  width="300"
                  height="480"
                  src="~/assets/images/accesories.svg"
                  alt="image slot"
                />
              </template>
            </b-carousel-slide>
            <b-carousel-slide>
              <template #img>
                <img
                  class="d-block center-block"
                  width="300"
                  height="480"
                  src="~/assets/images/speed-improve.svg"
                  alt="image slot"
                />
              </template>
            </b-carousel-slide>
            <b-carousel-slide>
              <template #img>
                <img
                  class="d-block center-block"
                  width="300"
                  height="480"
                  src="~/assets/images/exhaust.svg"
                  alt="image slot"
                />
              </template>
            </b-carousel-slide>
          </b-carousel>
        </div>
      </b-row>
      <p style="text-align: center; color: white"></p>
      <p style="text-align: center;">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis euismod
        libero vel leo auctor, in venenatis nulla consequat. Sed commodo nunc
        sit amet congue aliquam.
      </p>
    </div>
  </section>
</template>
<script>
export default {
  data: () => ({
    title: 'OUR SPECIALITY',
    copyright: 'Copyright © 2021 Company',
    description:
      'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis euismod libero vel leo auctor, in venenatis nulla consequat. Sed commodo nunc sit amet congue aliquam.',
    slide: 0,
    sliding: null,
  }),
}
</script>

<style>
.carousel-control-next,
.carousel-control-prev /*, .carousel-indicators */ {
  filter: invert(100%);
}
.carousel-item {
  background-position: center;
}
</style>
