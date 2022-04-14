<template>
  <div class="intro">
    <div class="intro-title">
      <img class="intro-photo" alt="Zihang logo" src="../assets/pig.png">
      <h1 id="full-name">Wang Zihang</h1>
    </div>
    <p>
      I'm a Web application developer.<br> Hope you can learn more about me from the blog.
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
  .intro {
    border: 5px solid lightblue;
  }

  img {
    float: right;
    margin-right: 20%;
    border-radius: 50%;
    width: 100px;
  }

  #full-name {
    margin: 150px 50px 25px 100px;
  }
  p {
    margin-left: 100px;
    margin-bottom: 25px;
  }
</style>
