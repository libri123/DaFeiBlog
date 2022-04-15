<template>
  <div class="topnav">
    <p class="name"><strong>zihang</strong></p>
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
  margin-top: 5px;
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
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
  margin-right: 10px;
}

.topnav .topnav-item:hover {
  background-color: #ddd;
}
</style>