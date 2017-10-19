<template lang="html">
  <section class="test">
    <div class="header">
      <img src="~/assets/images/profile.jpg" alt="Guy Lyons" class="profile">
      <h1 class="title">Guy Lyons</h1>
      <h2 class="subhead">Open Source Developer,<br/> Proponent, Advocate<br /> and Illustrator 🤓</h2>
      <div><nuxt-link to="/contact" class="tag">for hire!</nuxt-link></div>
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
  margin-bottom: 15px;
  padding: 2em;
  border: 2px solid #eee;
  border-radius: 5px;
  text-align: center;
  h1 {
    font-size: 30px;
    margin-bottom: 15px;
    text-transform: uppercase;
  }
}

.profile {
  border-radius: 50px;
  width: 100px;
  height: auto;
}

.tag {
  position: absolute;
  top: 10px;
  right: 10px;
  background: rgb(236, 54, 54);
  padding: 5px;
  border-radius: 20px;
  color: #fff;
  font-size: 9px;
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
