<template>
  <main>
    <div class="container">
      <div class="row">
        <div class="col">
          <ul>
            <li><a href="https://github.com/guylyons" class="button">Github</a></li>
            <li><a href="https://twitter.com/yugsnoyl" class="button">Twitter</a></li>
            <li><a href="https://www.linkedin.com/in/guylyons/" class="button">LinkedIn</a></li>
            <li><a href="mailto:that.guy@mailhero.io" class="button">Email</a></li>
          </ul>
        </div>
        <div class="col">
          <div class="ugly-ted">
            <img src="~assets/images/ugly-ted.png" alt="Ugly Ted" title="Don't hover over me!" width="300" height="auto">
          </div>
        </div>
      </div><!-- .row -->
      
      <div class="row col">
        <div class="copyright">
          <p>Guy Lyons ©2017</p>
        </div>
      </div>
    </div>
  </div>
</main>
</template>

<script>
import Header from "../components/Header.vue";
import "./index.scss";
import axios from "axios";

export default {
  data: function() {},
  async asyncData() {
    const { data } = await axios.get(
      "https://hacker-news.firebaseio.com/v0/topstories.json?print=pretty"
    );
    return { stories: data };
  }
};
</script>