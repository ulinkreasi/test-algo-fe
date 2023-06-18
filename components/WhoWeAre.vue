<template>
  <section id="who-we-are" style="overflow: hidden;">
   
    <div
      class="d-flex flex-column align-items-center bg-white cover p-4"
      style="min-height: 300px"
    >
      <div class="d-flex justify-content-center">
        <h1 style="color: #029fe4">{{ items[initial].title }}</h1>
        <div class=""></div>
      </div>
      <div class="p-2 border;font-weight:bold;font-size:18px">
        <h3>{{ items[initial].subtitle }}</h3>
        <p>
          {{ items[initial].content }}
        </p>
      </div>
    </div>
    <b-row>
      <b-col>
        <p>
          <strong>0{{ initial + 1 }}</strong
          >/0{{ maxlength + 1 }}
        </p>
      </b-col>
      <b-col style="overflow: hidden">
        <div style="float: right; overflow: hidden">
          <b-img
            @click="deCreaseInitial()"
            style="background-color: #f1f1f1"
            class="p-2"
            :src="require('~/assets/images/arrow-left.svg')"
          ></b-img>
          <b-img
            @click="inCreaseInitial()"
            style="background-color: #1ba0e1"
            class="p-2"
            :src="require('~/assets/images/arrow-right.svg')"
          ></b-img>
        </div>
      </b-col>
    </b-row>
  </section>
</template>

<script>
export default {
  methods: {
    inCreaseInitial() {
      if (this.initial < this.maxlength) {
        this.initial++
      }
    },
    deCreaseInitial() {
      if (this.initial > 0) {
        this.initial--
      }
    },
  },
  data: () => ({
    initial: 0,
    maxlength: 2,
    items: [
      {
        title: 'Who We Are',
        subtitle: 'Technology Company',
        content:
          'Sed ut perspiciatis unde omnis iste natus sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.',
      },
      {
        title: 'What we do',
        subtitle: 'Professional Brand Management',
        content:
          'Sed ut perspiciatis unde omnis iste natus sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.',
      },
      {
        title: 'How we do',
        subtitle: 'Strategize, Design, Collaborate',
        content:
          'Sed ut perspiciatis unde omnis iste natus sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.',
      },
    ],
  }),
}
</script>
<style>
.cover {
  min-height: 200px;
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}
</style>
