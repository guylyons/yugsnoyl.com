<template lang="html">
  <div class="container">
    <Header />
    <nuxt/>
    <Bottom />
  </div>
</template>

<script>
import Header from "../components/Header.vue";
import Bottom from "../components/Bottom.vue";

export default {
  components: {
    Header,
    Bottom
  },
  head: {
    title: "Guy Lyons"
  }
};
</script>
