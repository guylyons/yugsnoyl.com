<template lang="html">
  <main>
    <div class="row col">
      <ul>
        <li><a href="https://github.com/guylyons" class="button">Github</a></li>
        <li><a href="https://twitter.com/yugsnoyl" class="button">Twitter</a></li>
        <li><a href="https://www.linkedin.com/in/guylyons/" class="button">LinkedIn</a></li>
        <li><a href="mailto:that.guy@mailhero.io" class="button">Email</a></li>
      </ul>
      <div class="ugly-ted">
        <img src="~assets/images/ugly-ted.png" alt="Ugly Ted" title="Don't hover over me!" width="550" height="auto">
      </div>
    </div><!-- .row -->

    <div class="row col">
      <div class="copyright">
        <p>Guy Lyons ©2017</p>
      </div>
    </div>
  </div>
</main>
</template>

<style global lang="scss">
body {
  font-family: "Source Code Pro", monospace;
  background-color: #fff;
}
ul {
  list-style: none;
  margin: 0;
  padding: 0;
}
.container {
  max-width: 600px;
}
.copyright {
  font-weight: 500;
  color: #666;
  font-size: 12px;
}
.title {
  color: #2599d5;
  font-size: 50px;
  margin: 0;
}
.subhead {
  font-size: 14px;
  margin: 0;
}
.ugly-ted {
  position: absolute;
  top: 0; right: 0;
  z-index: -1;
}
.button {
  position: relative;
  border: 2px solid #e4e4e4;
  color: #111;
  text-decoration: none;
  padding: 15px 35px;
  margin-bottom: 15px;
  font-weight: 500;
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 1;
  background: rgba(255,255,255,0.7);
  &:hover {
    border-color: #111;
    text-decoration: none;
    color: #2599d5;
  }
  &::before {
    content: "";
    position: absolute;
    top: 8px;
    bottom: 8px;
    left: 20px;
    right: 20px;
    background-color: #fee94e;
    z-index: -1;
  }
}
.nuxt-link-exact-active {
  background: #ddd;
}
</style>

<script>
</script>
