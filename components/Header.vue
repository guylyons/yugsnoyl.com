<template lang="html">
  <section class="test">
    <div class="header">
      <img src="~/assets/images/profile.jpg" alt="Guy Lyons" class="profile">
      <h1 class="title">Guy Lyons</h1>
      <h2 class="subhead">Open Source Developer, Proponent, Advocate &amp; Illustrator 🤓</h2>
      <div><a href="mailto:that.guy@mailhero.io" class="tag">for hire!</a></div>
    </div>

    <nav class="nav nav-main">
      <nuxt-link to="/">Home</nuxt-link>
      <!-- <nuxt-link to="/work">Work</nuxt-link> -->
      <nuxt-link to="/find-me">Find Me</nuxt-link>
    </nav>
  </section>
</template>

<style scoped lang="scss">
.header {
  position: relative;
  margin-top: 15px;
  padding: 2em;
  text-align: center;
  h1 {
    font-size: 25px;
    font-weight: bold;
    margin-top: 10px;
    margin-bottom: 10px;
    text-transform: uppercase;
  }
}

.profile {
  border-radius: 50px;
  width: 100px;
  height: auto;
}

.tag {
  padding: 3px 8px;
  border-radius: 20px;
  color: #fff;
  font-size: 13px;
  display: inline-block;
  background: rgb(236, 54, 54);
  &:hover {
    background: darken(rgb(236, 54, 54), 20%);
  }
  text-decoration: none;
}

.nav {
  display: flex;
}
.nav {
  display: flex;
  background: #eee;
  border-radius: 3px;
  overflow: hidden;
  margin-bottom: 15px;
  justify-content: center;
  align-items: center;
  a {
    flex-grow: 1;
    text-align: center;
    padding-top: 15px;
    padding-bottom: 15px;
    border: 2px solid transparent;
    &:hover {
      background: #ddd;
    }
    &:active {
      border: 2px solid #666;
    }
  }
}
  </style>
