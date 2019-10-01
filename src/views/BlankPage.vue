<template>
   <div>
    <div class="container-fluid">
        <nav aria-label="breadcrumb">
            <div>
              <h1 class="title-6">BLANK PAGE</h1>
              <ul class="lists-6">
                <li> <a href="#" class="home">  Home</a>  </li>
                <li> <a href="#" class="db">  >  Blankpage  </a>  </li>
              </ul>
            </div>
        </nav>
    </div>
      <div class="container" style="margin-top:20px;">
        <div class="card">
          <div class="card-body" style="margin-top:50px;">
            <a href="#create"><i class="fa fa-plus-circle"  style="font-size:180px;" aria-hidden="true"></i></a>
          </div>
          <p href="" style="font-size:40px;">Create your own page.</p>
        </div>
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
 .title-6 {
    padding-right: 889px;
    font-size: 30px;
    margin-top: 16px;
 }
 
 .container-fluid {
   background:rgb(231, 224, 224);
   top: 0%;
   margin-top: -20px;
 }
 .lists-6 {
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
   .title-6  {  
    margin-left: 150px;
   }
   .lists-6 {
     padding-left: 150px;
   }
 }
</style>