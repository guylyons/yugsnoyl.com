<template lang="html">
    <div>
        <h1>Posts</h1>
        <ul>
          <li v-for="post in posts">
            <nuxt-link :to="{ name: 'posts-id', params: { id: post.id } }">{{ post.title }}</nuxt-link>
        </li>
    </ul>
    </div>
</template>

<style lang="scss">

</style>

<script>
import axios from 'axios'

export default {
  asyncData ({ req, params }) {
    // We can return a Promise instead of calling the callback
    return axios.get('https://jsonplaceholder.typicode.com/posts')
    .then((res) => {
      return { posts: res.data.slice(0, 5) }
    })
  },
  head: {
    title: 'List of posts'
  }
}
</script>
