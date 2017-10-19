<template lang="html">
    <div>
        <p>Posts ({{posts.length}})</p>
        <ul>
          <li v-for="post in posts">
            <h1 class="post-title">{{ post.title.rendered }}</h1>
            <!-- <div v-html="post.content.rendered"></div> -->
        </li>
    </ul>
    </div>
</template>

<style scoped lang="scss">
.post-title {
  font-size: 18px;
  border-bottom: 2px solid #ddd;
  margin-bottom: 15px;
  background: #eee;
}
</style>

<script>
import axios from "axios";

export default {
  asyncData({ req, params }) {
    return axios.get("https://csartmaine.org/wp-json/wp/v2/posts").then(res => {
      return { posts: res.data };
    });
  },
  head: {
    title: "List of posts"
  }
};
</script>
