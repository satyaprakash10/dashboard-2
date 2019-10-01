<template>
  <div  id="mySidenav" class="sidebar">
    <!-- <div class="formation"> -->
      <router-link to="/">
        <li><a href="# "><i class="fa fa-tachometer" aria-hidden="true" style="padding:7px;"></i> DASHBOARD</a></li>
      </router-link>

      <router-link to="/profile">
         <li><a href="# " class="active" style="padding-right: 97px;"><i class="fa fa-user" style="padding:8px;" aria-hidden="true"></i> FORM</a></li>
      </router-link>

      <router-link to="/basic">
         <li><a href="# " style="padding-right: 47px;"><i style="padding:8px;" class="fa fa-table" aria-hidden="true"></i>  BASIC TABLE </a></li>
      </router-link>

      <router-link to="/icons">
         <li><a href="# "  style=" padding-right:98px;"><i class="fa fa-grav" style="" style="padding:8px;" aria-hidden="true"></i> ICONS</a> </li> 
      </router-link>

      <router-link to="/Google">
        <li><a href="#" style=" padding-right: 47px;"><i class="fa fa-globe" style="padding:9px;" aria-hidden="true"></i>GOOGLE MAP</a></li>
      </router-link>

      <router-link to="/blankpage">
        <li><a href="#" style="padding-right: 57px;"><i class="fa fa-exclamation-circle" style="padding:9px;" aria-hidden="true"></i>BLANK PAGE</a></li>
      </router-link>
      
      <router-link to="/error">
        <li><a href="# " style=" padding-right: 67px;"><i class="fa fa-exclamation-triangle" style="padding:8px;" aria-hidden="true"></i> ERROR 404</a></li>     
      </router-link>
      
      <router-link to="/form">
      <li><a href="# " style="padding-right: 92px;"><i style="padding:8px;"  class="fa fa-address-book"" aria-hidden="true"></i> PROFILE</a></li>     
    </router-link>
    <!-- </div> -->
    <button class="btnn btn-warning" style= "font-size:15px">Upgrade to Pro</button>
  </div>
</template>
<script>
export default {
    
}
</script>
<style>
.sidebar {
  margin: -21px;
  width: 250px;
  background-color: #4337a4;
  position: fixed;
  padding-top: 10px;
  height: 100%;
  list-style: none;
  overflow: hidden;
  display: block;
  color:  #b6b3cc;
  padding: 1px;
  z-index: 1;
  /* padding-top: 64px; */
  text-decoration: none;
  transition: .3s;
}

.sidebar li a {
    display: block;
    font-size: 17px;
    color: #b6b3cc;
    padding: 15px 34px 20px 18px;
    text-decoration: none;
}
 
.sidebar li a:hover:not(.active) {
  background-color: #b6b3cc;
  color: white;
}

.icons-bar {
  display: none;
}
 

  
@media screen and (max-width: 768px) {
  .sidebar {
    left: -355px;
    display: block;
    z-index: 30;
    padding-top: 4px;

  }
  .icons-bar {
    display: block;
    margin-left: 10px;
    font-size: 30px;
  }
  .sidebar li a {
    display: flex;
    justify-content: center;
    padding:  2px 37px 30px 21px;
  }
  .sidebar-image {
    display:block;
    /* margin-left: 20px; */
  }
  .dropdown {
    display: block;
    margin-left: 160px;
  }
}
  
 
@media screen and (max-width:960px)
{
 .sidebar-image {
   display: none;
 }
 
}
</style>