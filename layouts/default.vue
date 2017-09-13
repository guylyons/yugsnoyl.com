<template>
  <div class="container">
    <div id="particles-js"></div>
    <Header />
    <nuxt/>
  </div>
</template>

<script>
import Header from "../components/Header.vue";

export default {
  components: {
    Header
  },
  head: {
    title: "Guy Lyons"
  }
};
</script>
