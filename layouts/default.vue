<template lang="html">
  <div class="container">
    <Header />
    <nuxt/>
    <Bottom />
  </div>
</template>

<script>
import Header from "../components/Header.vue";
import Footer from "../components/Footer.vue";

export default {
  components: {
    Header,
    Footer
  },
  head: {
    title: "Guy Lyons - Developer"
  }
};
</script>
