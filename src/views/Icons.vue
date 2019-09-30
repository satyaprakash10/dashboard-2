<template>
  <div>
    <div class="container-fluid">
        <!-- <nav aria-label="breadcrumb"> -->
            <div>
              <h1 class="title-4">ICONS </h1>
              <ul class="lists-4">
                <li> <a href="#" class="home">  Home</a>  </li>
                <li> <a href="#" class="icons">  >  Icons  </a>  </li>
              </ul>
            </div>
        <!-- </nav> -->
    </div>
    <h1>Our Services</h1>
    <div class="container">
      <div class="row services">
        <div class="col-md-4 text-center">
            <div class="icon">
              <i class="fa fa-tablet"></i>
            </div>
            <h3>App Development</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Voluptate obcaecati consectetur maxime repellat quisquam itaque voluptatibus 
              saepe, dolorum neque placeat veritatis tenetur iure nemo velit minima ducimus
              necessitatibus ad error?</p>
          </div>
          <div class="col-md-4 text-center">
              <div class="icon">
                <i class="fa fa-line-chart"></i>
              </div>
              <h3> Graphic Design</h3>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Voluptate obcaecati consectetur maxime repellat quisquam itaque voluptatibus 
                saepe, dolorum neque placeat veritatis tenetur iure nemo velit minima ducimus
                necessitatibus ad error?</p>
            </div>
            <div class="col-md-4 text-center">
              <div class="icon">
                <i class="fa fa-paint-brush"></i>
              </div>
              <h3>Digital MArketing</h3>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Voluptate obcaecati consectetur maxime repellat quisquam itaque voluptatibus 
                saepe, dolorum neque placeat veritatis tenetur iure nemo velit minima ducimus
                necessitatibus ad error?</p>
          </div>
        </div>     
     </div>
  </div>
</template>
<script>
export default {
    
}
</script>
<style>
 
 .title-4 {
    padding-right: 980px;
    font-size: 30px;
    margin-top: 18px;
 }
 
 .container-fluid {
   background:rgb(231, 224, 224);
   top: 0%;
   /* margin-top: -20px; */
 }
 .lists-4 {
   list-style: none;
   padding-left: 255px;
   display: flex;
   text-decoration: none;
   font-size: 15px;
   flex-wrap: nowrap;
 }
 .home {
   color: rgb(79, 50, 211);
   padding-right: 10px;
 }
 .icons {
   color: grey;
 }

 .services {
  /* background-image: linear-gradient(rgba(0,0,0,0.8)),url(1.jpg);0 */
  background-image: linear-gradient(rgba(77, 70, 70, 0.8),rgba(97, 92, 92, 0.8));
  background-size: center;
  color: #eeffee !important;
  background-attachment: fixed;
  padding-top: 50px;
  padding-bottom: 50px;
}

.services h1::after {
  content: '';
  background: #eeffee;
  display: block;
  height: 3px;
  width: 170px;
  margin: 20px auto 5px;
}

.services {
   margin-top: 40px;
}

.icon {
  font-size: 40px;
  margin: 20px auto;
  padding: 20px;
  height: 80px;
  width: 80px;
  border:1px solid #fff;
  border-radius: 50%;
}

.services p {
  font-size: 14px;
  margin-top: 20px;
  color: #ccc;
}

.services .col-md-3:hover {
  background: #167bda;
  cursor: pointer;
  transition: 0.7s;
}
</style>