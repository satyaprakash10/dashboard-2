<template>
  <div>
    <div class="container-fluid">
        <nav aria-label="breadcrumb">
            <div>
              <h1 class="title-5">GOOGLEMAP</h1>
              <ul class="lists-5">
                <li> <a href="#" class="home">  Home</a>  </li>
                <li> <a href="#" class="db">  >  Google map  </a>  </li>
              </ul>
            </div>
        </nav>
    </div>
    <div class="container map-sect" style="margin-top:20px;">
      <h1>Map Overview..<span style="font-size:12px;">Check your place/Loaction</span></h1>
      <hr>
      <div class="card-body">
        <!-- <div class="row">
          <div class="col-md-12"> -->
            <img class="card-img-top" :src="image" alt="Card image cap" style="width: 100%; height: 500px;">
          <!-- </div>
        </div> -->
      </div>
       <!-- <div class="card-body" >
        <a href=""> <img :src="image" class="map-style"style="position:relative;"  alt="map"> </a>
      </div> -->
    </div>

  </div>
</template>
<script>
import image from "../assets/map.jpg"
export default {
    data()
  {
    return{
      // images: {
      //   sample: 'assets/sample.jpg'
      // }
     image: image
    }
  }
}
</script>
<style>
 body {
   overflow-x: hidden;
 }
 /* .map-sect {
   position: relative;
 } */
.title-5 {
  padding-right: 880px;
  font-size: 30px;
  margin-top: 16px; 
}
 
.container-fluid {
  background:rgb(231, 224, 224);
  top: 0%;
  margin-top: -20px;
  /* position: relative; */
}
.lists-5 {
  list-style: none;
  padding-left: 245px;
  display: flex;
  text-decoration: none;
  font-size: 15px;
  flex-wrap: nowrap;
}
.home {
  color: rgb(79, 50, 211);
  padding-right: 10px;
}
.db {
  color: grey;
}
.map-style {
  margin-top: 20px;
  height: 500px;
  width: 1000px;
  position: relative;
}

 @media screen and (max-width: 780px) {
   .title-5  {  
    margin-left: 120px;
   }
   .lists-5 {
     padding-left: 125px;
   }
 }
</style>