<template>
  <div class="flex">
    <div class="left">
      <header class="row">
        <h1 class="title">Guy Lyons</h1>
        <h2 class="subhead">Web Dev &amp; Design</h2>
        <div class="mugshot">
          <img src="~assets/images/guy.png" alt="Guy Lyons" title="Hire me!">
        </div>
      </header>
    </div>
    <div class="right">
      <ul>
        <li><a href="https://github.com/guylyons" class="button">Github</a></li>
        <li><a href="#" class="button">Twitter</a></li>
        <li><a href="https://www.linkedin.com/in/guylyons/" class="button">LinkedIn</a></li>
        <li><a href="mailto:that.guy@mailhero.io" class="button">Email</a></li>
      </ul>
      <div class="ugly-ted">
        <img src="~assets/images/ugly-ted.png" alt="Ugly Ted" title="Don't hover over me!" width="300" height="auto">
      </div>
      <div class="copyright row">
        <p>Guy Lyons ©2017</p>
      </div>
    </div>
  </div>
</template>

<script>
// import Header from '../components/Header.vue'

export default {
  data: () => {
    return { name: 'world' }
  },
  components: {
    // Header,
  }
}
</script>

<style lang="scss">
html,
body {
  height: 100%;
}
* {
  box-sizing: border-box;
}
body {
  margin: 0;
  padding: 0;
  font-family: "Atlas Grotesk";
}
ul {
  list-style: none;
  margin: 0;
}
.flex {
  display: flex;
  @media (max-width: 540px) {
    flex-direction: column;
    text-align: center;
  }
}
.left,
.right {
  position: relative;
  display: inherit;
  flex: 1;
  justify-content: center;
  flex-grow: 1;
  height: 100vh;
  padding: 2em;
}
.left {
  background-color: #EEE;
  flex-direction: column;
  text-align: right;
}
.copyright {
  font-weight: 500;
  color: #666;
  font-size: 10px;
}
.right {
  flex-direction: column;
  background-color: #FFF;
  text-align: center;
}
.title {
  color: #2599D5;
  font-size: 50px;
  margin: 0;
}
.subhead {
  font-size: 14px;
  margin: 0;
}
.button {
  position: relative;
  border: 2px solid #E4E4E4;
  color: #000;
  text-decoration: none;
  padding: 10px 35px;
  display: block;
  text-align: center;
  margin-bottom: 15px;
  font-size: 20px;
  font-weight: 500;
  z-index: 20;
  max-width: 200px;
  margin-left: auto;
  margin-right: auto;
  &:hover {
    border-color: #000;
  }
  &::before {
    content: "";
    position: absolute;
    top: 8px; bottom: 8px;
    left: 20px; right: 20px;
    background-color: #FEE94E;
    z-index: -1;
  }
}
</style>
