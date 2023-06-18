<template>
  <header>
    <b-navbar toggleable type="white" variant="white">
      <b-navbar-brand href="#">
        <b-img
          class="ml-5"
          style="min-height: 50px"
          alt="Image Company"
          :src="require('~/assets/images/company-blue.svg')"
        />
      </b-navbar-brand>

      <b-navbar-toggle target="navbar-toggle-collapse">
        <template #default="{ expanded }">
          <b-icon name="x" v-if="expanded" icon="chevron-bar-up"></b-icon>
          <b-img v-else :src="require('~/assets/images/burger.svg')"></b-img>
        </template>
      </b-navbar-toggle>

      <b-collapse id="navbar-toggle-collapse" is-nav>
        <b-navbar-nav class="ml-auto">
          <b-nav-item href="#">Link 1</b-nav-item>
          <b-nav-item href="#">Link 2</b-nav-item>
          <b-nav-item href="#" disabled>Disabled</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </header>
</template>
<script>
export default {
  data: () => ({
    expanded: true,
  }),
}
</script>
<style></style>
