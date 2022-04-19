<template>
  <div class="topnav">
    <p class="name"><strong>zihang</strong></p>
    <button class="download"><a download href="downloads/example.txt">Download CV</a></button>
    <router-link to="/gallary" class="topnav-item">Gallary</router-link>
    <router-link to="/article" class="topnav-item">Article</router-link>
    <router-link to="/" class="topnav-item">Home</router-link>
  </div>
</template>
<script>
  export default {
    name: 'Nav',
  };
</script>
<style scoped>
.topnav {
  overflow: hidden;
  width: 100%;
  border: 5px solid lightblue;
}

.topnav .name {
  position: relative;
  float: left;
  margin-left: 5%;
  color: #0d8ba1;
}

.topnav .topnav-item {
  float: right;
  text-align: center;
  padding: 18px 16px;
  text-decoration: none;
  font-size: 17px;
  margin-right: 10px;
}

.topnav .topnav-item:hover {
  background-color: #ddd;
}

.download {
  color: #bfbfbf;
  background: none;
  border: 1px #0d8ba1 solid;
  border-radius: 1000px;
  padding: 10px;
  -webkit-transition: border-color 0.3s ease;
  -o-transition: border-color 0.3s ease;
  transition: border-color 0.3s ease;
  cursor: pointer;
  float: right;
  margin-top: 0.5%;
  margin-right: 0.5%;
}
.download a {
    font-size: 17px; 
}
.download:hover {
  border-color: #bfbfbf; 
}
</style>