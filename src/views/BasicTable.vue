<template>
  <div class="container-fluid">
      <!-- <nav aria-label="breadcrumb"> -->
          <div class="title">
            <h1>BASIC TABLE</h1>
             <ul class="lists">  
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
 .title {
    padding-right: 941px;
    margin-top: 27px;
    font-size: 30px;
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
   margin-top: -18px;
 }
 .lists {
   list-style: none;
   /* padding-left: 285px; */
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
</style>