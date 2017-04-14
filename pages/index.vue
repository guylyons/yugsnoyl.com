<template>
  <main>
    <div class="container">
      <Header></Header>
      <div class="row text-center">
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
    </div>
  </main>
</template>

<script>
import Header from '../components/Header.vue'

export default {
  data: function() {
    return { name: 'world' }
  },
  components: {
    Header,
  },
  head: {
    title: "Guy Lyons - Dev & Design"
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
.container {
  max-width: 500px;
}
.copyright {
  font-weight: 500;
  color: #666;
  font-size: 10px;
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
.ugly-ted {
  text-align: right;
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
  font-size: 16px;
  font-weight: 500;
  z-index: 20;
  max-width: 200px;
  margin-left: auto;
  margin-right: auto;
  &:hover {
    border-color: #000;
    text-decoration: none;
    color: #2599D5;
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
