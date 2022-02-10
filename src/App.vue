<template>
  <v-app class="app">
    <v-app-bar color="green" app>
      <v-app-bar-nav-icon>
      </v-app-bar-nav-icon>
      <v-app-bar-title>
        Review
      </v-app-bar-title>
    </v-app-bar>

    <v-main>
      <v-container>
          <review-list :reviews="reviews"/>
      </v-container>
    </v-main>

    <v-footer>
      All rights reserved
    </v-footer>
  </v-app>
</template>

<script>
import ReviewList from "./components/ReviewList";

export default {
  name: 'App',

  components: {
    ReviewList
  },

  data() {
    return {
      reviews: [
        {id: 1, name: 'КК', img: 'https://tr-static.eodev.com/files/d33/d683361ac68323c827b9bef615640901.jpg'},
        {id: 2, name: 'ОИ', img: 'https://i.pinimg.com/736x/bb/03/5a/bb035a9f1fc50e4cfc3f58a4e0ab9494.jpg'},
        {id: 3, name: 'ВЧ', img: 'https://p.favim.com/orig/2019/04/13/spring-bunny-yes-Favim.com-7086897.jpg'},
      ],
    }
  },
};
</script>

<style>
.app {
  background-color: #F5F5FA !important;
}
</style>
