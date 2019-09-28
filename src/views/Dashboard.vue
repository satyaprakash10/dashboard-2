<template>
  <div class="container-fluid seconadary">
      <nav aria-label="breadcrumb">
          <div>
            <h1 class="title">Dashboard</h1>
            <ul class="lists">
              <li><a href="#" class="home">  Home</a></li>
              <li><a href="#" class="db">  >  Dashboard</a></li>
            </ul>
             <button class="btn btn-danger upgradebtn">Upgrade to pro</button>
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
 .title {
    padding-right: 946px;
    font-size: 30px;
 }
.upgradebtn {
    float: right;
    font-size: 20px;
    margin-top: -63px;
}
 .seconadary {
   background:rgb(231, 224, 224);
   top: 0%;
   margin-top: -20px;
 }
 .lists {
   list-style: none;
   padding-left: 248px;
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

 @media screen and(max-width:375px) {
   .title {
     margin-left: 100px;
   }
   .lists {
     margin-right: -146px;
   }
 }
</style>