<template>
  <div>
    <div class="container-fluid">
        <nav aria-label="breadcrumb">
            <div>
              <h1 class="title-7">ERROR 404</h1>
              <ul class="lists-7">
                <li> <a href="#" class="home">  Home</a>  </li>
                <li> <a href="#" class="db">  >  Error 404..  </a>  </li>
              </ul>
            </div>
        </nav>
    </div>
    <div class="card">
       <div class="card-header">
         <h1 style="color:red;">Error Found..<span style="font-size:14px; color:grey;">The page is not working..</span></h1>
       </div>
       <!-- <div class="row"> -->
        <!-- <div class="col-md-8"> -->
          <div class="car-body" style="margin-top:30px;">
            <i class="fa fa-exclamation-triangle" style="font-size: 178px;" aria-hidden="true"></i>
          </div>
        <!-- </div> -->
       <!-- </div> -->
    </div>

  </div>
</template>
<script>
export default {
    
}
</script>
<style>
 /* .breadcrumb {
 } */
 .title-7 {
    padding-right: 908px;
    font-size: 30px;
    margin-top: 16px;
 }
  
 .container-fluid {
   background:rgb(231, 224, 224);
   top: 0%;
   margin-top: -20px;
 }
 .lists-7 {
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
  @media screen and (max-width: 780px) {
   .title-7  {  
    margin-left: 150px;
   }
   .lists-7 {
     padding-left: 150px;
   }
 }
</style>