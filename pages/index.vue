<template>
  <main>
    <div class="container">
      <div class="row text-center">
        <div class="col left">
          <header>
            <h1 class="title">Guy</h1>
            <h2 class="subhead">Web Dev &amp; Design</h2>
            <div class="mugshot">
              <img src="~assets/images/guy.png" alt="Guy Lyons" title="Hire me!">
            </div>
          </header>
        </div>
        <div class="col right">
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
    </div>
  </main>
</template>

<script>
// import Header from '../components/Header.vue'

export default {
  data: function() {
    return { name: 'world' }
  },
  components: {
    // Header,
  },
  head: {
    title: "Guy Lyons - Web Dev & Design"
  }
}
</script>

<style lang="scss">
body {
  font-family: "Atlas Grotesk";
}
ul {
  list-style: none;
  margin: 0;
}
.left {
  background-color: #EEE;
}
.copyright {
  font-weight: 500;
  color: #666;
  font-size: 10px;
}
.right {
  background-color: #FFF;
  ul {padding: 0;}
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
