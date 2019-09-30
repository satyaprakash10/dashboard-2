<template>
    <div>
         <nav class="navbar navbar-expand-md  bg-primary">
           <i class="fa fa-viacoin logo-style-1" aria-hidden="true"></i>
            <a href="#" class=" logo-style">MATERIALPRO.</a>
            <div class="collapse-menu">
              <div class="collapse-menu-icon-container">
                <a href="javascript:void(0)"  @click="myFunction()"><i class="fa fa-bars icons-bar" aria-hidden="true"></i></a>
              </div>
            </div>
             <!-- <button  class="fa fa-search btn button-style"></button> -->
            <div class="collapse navbar-collapse justify-content-between" id="navbarCollapse">
              
            </div>
             <div class="nav-profile">
             <a href=""> <img :src="image" class="sidebar-image"/></a>      
             </div>
              <h3><a href="" class="profile-pic">Alex Costa</a></h3>
          
      </nav>
    </div>
</template>

<script>
import image from "../assets/sample.jpg"

export default {
  components:{

  },
  data()
  {
    return{
      
     image: image
    }
  },
  methods:
  {
    myFunction() {
      let showhide = document.getElementById('mySidenav');
      
      if(showhide.style.left === "-250px"){
          showhide.style.left = "0px";
      } else {
          showhide.style.left = "-250px";
      }
      }
}
}
 
</script>

<style >
body {
  margin: 0;
  font-family: "Lato", sans-serif;
  background: #efefef;
}
 
.profile-pic {
  font-size: 25px;
  text-decoration: none;
  color: white;
}
.h3 a:hover {
  color: bisque;
  text-decoration: none;
}

.icons-bar {
  font-size: 40px;
  margin-right: 34px;
  color: white;
}
.navbar { 
  position: fixed;
  z-index: 100;
  width: 100%;
}
.button-style {
  margin-left: 10px;
  color: white;
  font-size: 20px;
}
.logo-style {
  font-size: 25px;
  color: white;
  margin-top: 13px;
  margin-bottom: 10px;
  text-decoration: none;
  margin-left: 10px;
}

.logo-style-1 {
  font-size: 25px;
}

.btn-style {
  color: white;
  /* margin-top: 55px; */
  font-size: 20px;
  margin-right: 5px;
}

.sidebar-image{ 
  border-radius:50%;
  width: 30px;
  height: 30px;  
  margin-top: 5px;
  overflow: hidden;
  margin-left: auto;
  margin-right: 16px;
  margin-top: -1px;
}

@media screen and (max-width: 768px) {
    
  .logo-style {
    padding-left: 60px;
  }
   .icons-bar {
    /* margin-left: 493px; */
    margin-right: 200px;
    margin-top: -45px;
    display: block;
    color: white;
   }
   .logo-style-1 {
    margin-bottom: -67px;
    margin-left: 311px;
   }   
   .button-style {
     display: none;
   }
   .sidebar-image {
     /* display: none; */
     margin-top: -45px;
     margin-left: 150px;
   }
   .profile-pic {
     display: none;
   }
   
}
  @media screen and (max-width: 400px) {
   .icons-bar {
    margin-left: 300px;
    margin-top: -48px;
   }
   .logo-style-1 {
    margin-bottom: -72px;
    margin-right: 132px;
   }   
   .button-style {
     display: none;
   }
   /* .sidebar-image {
     display: none;
   } */
   .profile-pic {
     display: none;
   }
}
 @media screen  and (max-width: 375px){
   .icons-bar {
    /* margin-left: 325px;  */
      padding-left: 21px;
   }
   .sidebar-image {
     display: none;
     margin-right: 18px;
     margin-top: -43px;
   }
 }

</style>