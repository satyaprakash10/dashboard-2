<template>
  <div>
     <div class="container-fluid seconadary mb-5">
      <nav aria-label="breadcrumb">
          <div>
            <div>
              <h1 class="title">PROFILE</h1>
              <ul class="lists">
                <li><a href="#" class="home" style="margin-left:10px;">  Home</a></li>
                <li><a href="#" class="db">  >  Profile</a></li>
              </ul>
            </div>
            <b-button variant="success" style="font-size:12px;" class="upgradebtn">Visit here</b-button>
             <!-- <button class="btn btn-danger upgradebtn">Upgrade to pro</button> -->
          </div>
      </nav>
  </div>  
    <div class="container">
      <h1>Our Experts.</h1>
      <P>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Illum quibusdam iure deleniti maiores iusto tenetur animi sit tempora fugiat laudantium quasi.</P>
       <hr>
      <div class="row">
        <div class="col-md-3">  
          <div class="card-body">
             <a href=""> <img :src="image" ></a>     
          </div>
          <div class="card-footer">
            <h2>Alex costa</h2>
            <p>WEB DESIGNER</p>
            <button class="btn btn-primary">Read More</button>
          </div>
        </div>
           <div class="col-md-3">  
          <div class="card-body">
             <a href=""> <img :src="image" ></a>     
          </div>
          <div class="card-footer">
            <h2>Alex costa</h2>
            <p>TESTER</p>
            <button class="btn btn-primary">Read More</button>
          </div>
        </div>
           <div class="col-md-3">  
          <div class="card-body">
             <a href=""> <img :src="image" ></a>     
          </div>
          <div class="card-footer">
            <h2>Alex costa</h2>
            <p>APP DEVELOPER</p>
            <button class="btn btn-primary">Read More</button>
          </div>
        </div>
           <div class="col-md-3">  
          <div class="card-body">
             <a href=""> <img :src="image" ></a>     
          </div>
          <div class="card-footer">
            <h2>Alex costa</h2>
            <p>Graphic designer</p>
            <button class="btn btn-primary">Read More</button>
          </div>
        </div>
      </div> 
    </div>
  </div>
</template>

<script>
import image from "../assets/sample.jpg"
export default {
    components: {

    },
     data()
  {
    return{
      
     image: image
    }
  }
}
</script>
<style >

 @media screen and (max-width: 780px) {
   .title-8  {  
     margin-right: 150px;
   }
   .lists-8 {
     padding-left: 150px;
   }
 }
</style>