<template>
  <div class="container-fluid">
      <nav aria-label="breadcrumb">
          <div>
            <h1 class="title-2">PROFILE</h1>
            <ul class="lists">
              <li> <a href="#" class="home">  Home</a>  </li>
              <li> <a href="#" class="db">  >  Profile  </a>  </li>
            </ul>
          </div>
      </nav>
  </div>
</template>
<script>
export default {
    
}
</script>
<style>
 /* .breadcrumb {
 } */
 .title-2 {
    padding-right: 946px;
    font-size: 30px;
    margin-top: 16px;;
 }
 
 .container-fluid {
   background:rgb(231, 224, 224);
   top: 0%;
   margin-top: -20px;
 }
 .lists {
   list-style: none;
   padding-left: 249px;
   display: flex;
   text-decoration: none;
   font-size: 15px;
   flex-wrap: nowrap;
 }
 .home {
   color: rgb(79, 50, 211);
   padding-right: 15px;
 }
 .db {
   color: grey;
 }
</style>