<template>
  <div id="banner" style="background-color: #4097db; position: relative">
    <b-row no-gutters>
      <b-col>
        <b-img
          :src="require('~/assets/images/banner-top.svg')"
          style="width: 100%;height: 100%"
        ></b-img>
      </b-col>
      <!-- <div class="d-flex align-items-center" style="background-color: #4097db"> -->
      <div class="col" style="background-color: #4097db">
        <div class="p-5 mt-4">
          <h1 style="color: white; font-size: xxx-large">
            Discover Your Wonder
          </h1>
          <p class="custom-font" style="color: white">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim veniam.
          </p>
        </div>
      </div>
    </b-row>
    <a href="#our-core-values">
      <div
        class="d-flex justify-content-center"
        style="position: absolute; left: 49%; bottom: -4px !important"
      >
        <b-img :src="require('~/assets/images/scroll.svg')"></b-img>
      </div>
    </a>
  </div>
</template>
<style>
.custom-font {
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 500;
}
</style>
