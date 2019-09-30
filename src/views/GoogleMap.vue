<template>
  <div>
    <div class="container-fluid">
        <nav aria-label="breadcrumb">
            <div>
              <h1 class="title-5">GOOGLE MAP</h1>
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
      <div class="card-body" style="width: 80rem;">
        <!-- <div class="row">
          <div class="col-md-12"> -->
            <img class="card-img-top" :src="image" alt="Card image cap">
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
 .map-sect {
   position: relative;
 }
.title-5 {
  padding-right: 880px;
  font-size: 30px;
  margin-top: 16px; 
}
.Breadcrumb {
  display: flex;
  margin-left: 130px;
  /* padding-left: 141px; */
  font-size: 20px;
  flex-wrap: nowrap;
  margin-top: -55px;
  padding: 2.75rem 14rem;
  margin-bottom: -2rem;
  list-style: none;
  background-color: #e9ecef;
  border-radius: 0.25rem;   
}
.container-fluid {
  background:rgb(231, 224, 224);
  top: 0%;
  margin-top: -20px;
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
}
</style>