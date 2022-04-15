<template>
  <div class="intro">
    <div class="intro-title">
      <img class="intro-photo" alt="Zihang logo" src="../assets/personalPhoto.jpg">
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
    height: 600px;
  }

  img {
    float: right;
    margin-right: 15%;
    border-radius: 50%;
    width: 300px;
  }

  #full-name {
    margin: 100px 50px 25px 100px;
  }
  p {
    margin-left: 100px;
    margin-bottom: 25px;
  }
</style>
