<template>
  <footer>
    <div class="d-flex p-5" style="background-color: #07477a">
      <b-col>
        <a href="#">
          <b-img :src="require('~/assets/images/company-white.svg')"></b-img>
        </a>
      </b-col>
      <b-col class="bg-white p-3">
        <b-form-select
          class="mb-4"
          v-model="selected"
          :options="options"
          style="color: #00537c; font-weight: bold"
        ></b-form-select>
        <p>
          Jl. Lembong No 8 Kel. Braga Kec. Sumur Bandung, Kota Bandung, Jawa
          Barat
        </p>
      </b-col>
      <b-col class="flex-column flex-lg align-items-end justify-content-end">
        <a class="colorcustom mb-3" href="#who-we-are">Who We Are</a> <br/>
        <a class="colorcustom mb-3" href="#our-values">Our Values</a> <br/>
        <a class="colorcustom mb-3" href="#our-values">The Perks</a>
      </b-col>
    </div>
  </footer>
</template>
<script>
export default {
  data: () => ({
    selected: 'TECHNOLOGY DEPARTMENT',
    options: [
      { value: 'TECHNOLOGY DEPARTMENT', text: 'TECHNOLOGY DEPARTMENT' },
    ],
  }),
}
</script>
<style>
.colorcustom {
  color: white;
}

a:hover {
  color: white;
}
</style>
