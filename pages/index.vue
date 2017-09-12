<template>
  <main>
    <div class="container">
      <Header></Header>
      <div class="col">
        <ul>
          <li><a href="https://github.com/guylyons" class="button">Github</a></li>
          <li><a href="https://twitter.com/yugsnoyl" class="button">Twitter</a></li>
          <li><a href="https://www.linkedin.com/in/guylyons/" class="button">LinkedIn</a></li>
          <li><a href="mailto:that.guy@mailhero.io" class="button">Email</a></li>
        </ul>
        <div class="ugly-ted">
          <img src="~assets/images/ugly-ted.png" alt="Ugly Ted" title="Don't hover over me!" width="300" height="auto">
        </div>
        <div class="copyright">
          <p>Guy Lyons ©2017</p>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
import Header from "../components/Header.vue";
import "./index.scss";

export default {
  data: function() {},
  components: {
    Header
  }
};
</script>