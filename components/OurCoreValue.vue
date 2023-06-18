<template>
  <section id="our-core-values">
    <b-row no-gutters>
      <b-col cols="6" class="p-3">
        <b-row no-gutters class="justify-content-center" align-content="center">
          <h1 style="color: #029fe4">{{ heading1 }}</h1>
        </b-row>
        <p>{{ content }}</p>
        <div class="p-2 mt-3">
          <b-row>
            <b-col cols="1">
              <b-img
                width="inherit"
                :src="require('~/assets/images/icon-dash.svg')"
              ></b-img>
            </b-col>
            <b-col>
              <h3>{{ items[0].title }}</h3>
              <p>{{ items[0].content }}</p>
            </b-col>
          </b-row>
          <b-row>
            <b-col cols="1">
              <b-img
                width="inherit"
                :src="require('~/assets/images/icon-dash.svg')"
              ></b-img>
            </b-col>
            <b-col>
              <h3>{{ items[1].title }}</h3>
              <p>{{ items[1].content }}</p>
            </b-col>
          </b-row>
          <b-row>
            <b-col cols="1">
              <b-img
                width="inherit"
                :src="require('~/assets/images/icon-dash.svg')"
              ></b-img>
            </b-col>
            <b-col>
              <h3>{{ items[2].title }}</h3>
              <p>{{ items[2].content }}</p>
            </b-col>
          </b-row>
        </div>
      </b-col>
      <b-col cols="6" style="overflow: hidden">
        <b-img
          style="width: inherit"
          :src="require('~/assets/images/core-values.svg')"
        ></b-img>
      </b-col>
    </b-row>
  </section>
</template>
<script>
export default {
  data: () => ({
    heading1: 'Our Core Values',
    content:
      'Ridiculus laoreet libero pretium et, sit vel elementum convallis fames. Sit suspendisse etiam eget egestas. Aliquet odio et lectusetiam sit. In mauris rutrum ac ut volutpat, ornare nibh diam. Montes, vitae, nec amet enim.',
    items: [
      {
        title: 'Dedication',
        content:
          '  Nam libero tempore, cum soluta nobis est eligendi optio cumquenihil impedit quo minus id quod maxime placeat.',
      },
      {
        title: 'Intellectual Honesty',
        content:
          ' Itaque earum rerum hic tenetur a sapiente delectus, ut aut reiciendis voluptatibus maiores alias conse.',
      },
      {
        title: 'Curiosity',
        content:
          '  At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque.',
      },
    ],
  }),
}
</script>
