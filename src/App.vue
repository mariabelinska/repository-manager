<template>
  <v-app>
    <div id="app">
      <NavBar />
      <v-content class="content">
        <router-view />
      </v-content>
      <v-footer app absolute color="deep-purple" height="35"> </v-footer>
    </div>
  </v-app>
</template>

<script>
import NavBar from '@/components/NavBar.vue';

export default {
  name: 'App',
  components: {
    NavBar,
  },
};
</script>

<style>
a {
  text-decoration: none;
}
.container {
  max-width: 600px;
}
h1 {
  margin-bottom: 15px;
  margin-top: 15px;
}
.content {
  margin-bottom: 35px;
}
</style>
