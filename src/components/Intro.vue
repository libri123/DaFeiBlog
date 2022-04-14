<template>
  <div class="intro">
    <div class="intro-title">
      <img alt="Zihang logo" src="../assets/pig.png" width="200px" height="200px">
      <h1>Welcome to Zihang's blog</h1>
    </div>
    <p>
      You can find all the things about me from this blog<br>
    </p>
  </div>
</template>

<script>
export default {
  name: 'intro',
  props: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .intro-title {
    text-align: center;
  }
  p {
    text-align: center;
  }
</style>
