<template>
  <div id="app">
    <!-- <navbar/> -->
		<!-- <sidebar/> -->
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> -->
    <!-- </div> -->
    <navbar/>
		<sidebar/>
    <router-view />   
  </div>
</template>

<script>

import navbar from "./components/Navbar";
import sidebar from "./components/Sidebar";


export default {
  components:{
    sidebar,
    navbar
  }
};
</script>

<style lang="scss">
@import './sass/app.scss';
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.main-section {
  margin-left: 232px;
  margin-top: 20px;
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

@media screen and (max-width: 768px) {
   
}
</style>
