<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
<ons-page class="page">
   <v-ons-toolbar>
      <div class="center">{{ title }}</div>
      <div class="right">
        <v-ons-toolbar-button>
          <ons-icon icon="ion-navicon, material: md-menu"></ons-icon>
        </v-ons-toolbar-button>
      </div>
    </v-ons-toolbar>
  <div class="page__background"></div>
  <div class="page__content">
    コンテンツ
    <TopNews msg='News!' />
    <ons-input></ons-input>
    <div>追加コンテンツ</div>
  </div>
  <ons-fab></ons-fab>
</ons-page>
    </p>
  </div>
</template>

<script>
// @ is an alias to /src
import TopNews from '@/components/TopNews.vue'

export default {
  name: 'Top',
  props: {
    msg: String
  },
  components: {
    TopNews
  },
    data() {
    return {
      title: 'My app'
    }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>

