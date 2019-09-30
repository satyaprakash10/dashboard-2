<template>
<div>
  <div class="container-fluid seconadary mb-5">
      <nav aria-label="breadcrumb">
          <div>
            <div>
              <h1 class="title">Dashboard</h1>
              <ul class="lists">
                <li><a href="#" class="home">  Home</a></li>
                <li><a href="#" class="db">  >  Dashboard</a></li>
              </ul>
            </div>
            <b-button variant="danger" style="font-size:12px;" class="upgradebtn">Upgrade to pro</b-button>
             <!-- <button class="btn btn-danger upgradebtn">Upgrade to pro</button> -->
          </div>
      </nav>
  </div>  
  <hr>
  <div class="container">
     <div class="col-md-9">
      <div class="card">
       <div class="card-header bg-white">
         <div class="header-style">
          <h1>Sales Overview</h1>
          <p class="color-a">Apple Admin Vs GooglePixel Admin.</p>   
         </div>
         <ul class="list-style">
           <li class="apple">Apple</li>
           <li class="gp">GooglePixel</li>
         </ul>
       </div>
     </div>
      <div class="card-body bg-grey">
        <LineChart
            :labels="[
              'Sunday',
              'Monday',
              'Tuesday',
              'Wednesday',
              'Thursday',
              'Friday',
              'Satuerday'
            ]"
            :values="[50, 100, 150, 200, 250, 300]"
          />       
      </div>
    </div>
    <div class="col-md-3">
      <div class="card">
        <div class="card-header  bg-white">
          <h1>Our Visitor.</h1>
          <p class="p-style">Different devices Used to vist.</p>
        </div>
        <div class="card-body">
          <DoughnutChart
              :labels="['January', 'February', 'March', 'April', 'May']"
              :values="[80, 70, 40, 20, 50]"
              :color="['blue', 'green', 'yellow']"
            />
       </div>
         <div class="card-footer">
            <div class="card-footer">
              <ul class="lists-1">
                <li>Apple</li>
                <li>Samsung</li>
              </ul>
              <ul class="lists-b">
                <li>GooglePixel</li>
              </ul>
            </div>
          </div>
      </div>
    </div>
  </div>
</div>
</template>
<script>
import LineChart from "../components/LineChart"
import DoughnutChart from "../components/DoughnutChart"
export default {
    components:
    {
      LineChart,
      DoughnutChart
    }
}
</script>
<style>
.header-style { 
  float: left;
  margin-top: 10px;
}
.color-a {
  color: grey;
  font-size: 12px;
  margin-left:0px;
}
.list-style {
  display: flex;
  margin-top: 11px;
  margin-right: 10px;
  justify-content: space-between;
  font-size: 15px;
  float: right;
}
.apple {
  margin-right: 30px;
  color: skyblue;
}
.gp {
  color: blue;
  /* margin-left:5px; */
}
.lists-1 {
  color: blue;
  display: flex;
  font-size: 15px;
  margin-right: 16px;
  justify-content: space-between;
  /* margin-left: 40px; */
}
.p-style {
  color: grey;
  font-size: 13px;
}
.lists-b {
  padding-left: 22px;
  color: aqua;
  font-size: 15px;
}
.upgradebtn {
  height: 40px;
  
  width: 100px;
}
 
 
 @media screen and(max-width:756px) {
   .title {
     margin-right: -10px;
   }
   .lists {
     margin-right: -146px;
   }
   .seconadary {
     position: relative;
     margin-right: 100px;
   }
 }
</style>