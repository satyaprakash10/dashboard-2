<template>
  <div id="app">
    <!-- <navbar/> -->
		<!-- <sidebar/> -->
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> -->
    <!-- </div> -->
    
    <layout></layout> 
    <router-view />
   
  </div>
</template>

<script>

// import navbar from "./components/Navbar";
import layout from "./components/Layout";

export default {
  components:{
    layout
    // navbardx
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
