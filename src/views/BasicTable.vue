<template>
  <div class="container-fluid">
      <!-- <nav aria-label="breadcrumb"> -->
          <div class="title-3">
            <h1>BASIC TABLE</h1>
             <ul class="lists-3">  
              <li> <a href="#" class="home">  Home</a></li>
              <li> <a href="#" class="db"> >  Baic table</a></li>
            </ul>
          </div>
      <!-- </nav> -->
  </div>
</template>
<script>
export default {
    
}
</script>
<style>
 /* .breadcrumb {
 } */
 .title-3 {
    margin-right: 910px;
    margin-top: 27px;
    font-size: 30px;
 }
 
 .container-fluid {
   background:rgb(231, 224, 224);
   top: 0%;
   margin-top: -18px;
 }
 .lists-3 {
   list-style: none;
   /* padding-left: 200px; */
   margin-right: 100px;
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

 @media screen and (max-width: 360px) {
   .title-3  {  
    margin-right: 0px;
   }
   .lists-3 {
     padding-left: 87px;
   }
 }
</style>