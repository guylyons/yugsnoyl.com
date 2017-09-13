<template lang="html">
  <section>
    <div class="header">
     <h1 class="title">Guy Lyons</h1>
     <h2 class="subhead">Dev &amp; Design</h2>
   </div>

   <nav class="nav nav-main">
     <nuxt-link to="/">Home</nuxt-link>
     <nuxt-link to="/about">About</nuxt-link>
     <nuxt-link to="/contact">Contact</nuxt-link>
   </nav>
 </section>
</template>

<style scoped lang="scss">
.header {
  padding: 2em 0;
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
