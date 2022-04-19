<template>
  <div class="intro">
    <span>
      <img class="intro-photo" alt="Zihang logo" src="../assets/personalPhoto.jpg">
    </span>
    <span class="intro-content">
        <h1 id="full-name">Wang Zihang</h1>
        <p>I'm a Web application developer.<br> Hope you can learn more about me from the blog.</p>
    </span>
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
    height: 700px;
  }

  img {
    float: right;
    margin-top: 5%;
    margin-right: 15%;
    border-radius: 50%;
    width:25%;
  }

  #full-name {
    margin: 10% 5% 3% 10%;
  }
  p {
    margin-left: 10%;
  }
  
</style>
