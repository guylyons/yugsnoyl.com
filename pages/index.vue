<template lang="html">
  <main>
    <div class="row col">
      <div class="content entry-content">
        <h1>Who's that Guy?</h1>
        <p>Who me? I'm a developer living and working in Portland, Maine.</p>
        <p>I am a frequent contributor to open source projects and love all things in the JavaScript ecosysytem.</p>
        <p>I've worked on large scale projects running the gammut: from a complete redesign for <a href="https://balletcenter.nyu.edu" target="_blank">NYU</a> to art direction and technical lead for <a href="https://csartmaine.org" target="_blank">CSArt Maine</a></p>
      </div>
    </div><!-- .row -->
  </main>
</template>

<style lang="scss">
.entry-content {
  h1 {
    font-size: 1.8em;
    margin-top: .5em;
    margin-bottom: 1em;
    padding-bottom: .5em;
    border-bottom: 2px solid #eee;
  }
  text-align: center;
  p {
    line-height: 1.6;
  }
  p:last-child {
    margin-bottom: 5em;
  }
}
</style>

<script>
export default {
  data: () => {
    return {
      color: "blue"
    };
  }
};
</script>
