<template lang="html">
  <section>
    <div class="header">
     <h1 class="title">yug snoyl</h1>
     <h2 class="subhead">super amazingness developer guy <span class="tag">for hire!</span></h2>
   </div>

   <nav class="nav nav-main">
     <nuxt-link to="/">Home</nuxt-link>
     <nuxt-link to="/about">About</nuxt-link>
     <nuxt-link to="/blog">Blog</nuxt-link>
     <nuxt-link to="/contact">Contact</nuxt-link>
   </nav>
 </section>
</template>

<style scoped lang="scss">
.header {
  padding: 2em 0;
}

.tag {
  background: red;
  padding: 2px;
  border-radius: 5px;
  color: #fff;
}

.nav {
  display: flex;
}
.nav {
  display: flex;
  background: #eee;
  margin-bottom: 15px;
  a {
    flex-grow: 1;
    text-align: center;
    &:hover {
      background: #ddd;
    }
  }
}
</style>
