<template>
  <div class="topnav">
    <router-link to="/" class="topnav-item">Home</router-link> 
    <router-link to="/about" class="topnav-item">About</router-link>
    <router-link to="/weiwei" class="topnav-item">WeiWei</router-link>
  </div>
</template>
<script>
  export default {
    name: 'Nav',
  };
</script>
<style scoped>
.topnav{
  overflow: hidden;
  margin-top: 5px;
  margin-bottom: 10px;
  width: 100%;
  text-align: center;
}

.topnav .topnav-item {
  float: left;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}

.topnav .topnav-item:hover {
  background-color: #ddd;
}
</style>