<template>
 <div>
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
    <div class="container">
      <h1 style="margin-top:20px; text-align:left;">WorkSheet..</h1>
      <table id="firstTable" style="margin-top:25px;">
        <thead>
          <tr>
            <th>ID</th>
            <th>Name</th>
            <th>Phone</th>
            <th>Profession</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>101.</td>
            <td>Alex</td>
            <td>+91012e28802 </td>
            <td>HR</td>
          </tr>
            <tr>
            <td>101.</td>
            <td>Alex</td>
            <td>+91012e28802 </td>
            <td>HR</td>
          </tr>
            <tr>
            <td>101.</td>
            <td>Alex</td>
            <td>+91012e28802 </td>
            <td>HR</td>
          </tr>
            <tr>
            <td>101.</td>
            <td>Alex</td>
            <td>+91012e28802 </td>
            <td>HR</td>
          </tr>
            <tr>
            <td>101.</td>
            <td>Alex</td>
            <td>+91012e28802 </td>
            <td>HR</td>
          </tr>
            <tr>
            <td>101.</td>
            <td>Alex</td>
            <td>+91012e28802 </td>
            <td>HR</td>
          </tr>
            <tr>
            <td>101.</td>
            <td>Alex</td>
            <td>+91012e28802 </td>
            <td>HR</td>
          </tr>
        </tbody>
    </table>
  </div>
 </div>
</template>
<script>
export default {
  // var :firstTable = new Vue({
  //   el: '#firstTable',
  //   data: {
  //     rows: [
  //       { id: 1, name: "Chandler Bing", phone: '305-917-1301', profession: 'IT Manager' },
  //       { id: 2, name: "Ross Geller", phone: '210-684-8953', profession: 'Paleontologist' },
  //       { id: 3, name: "Rachel Green", phone: '765-338-0312', profession: 'Waitress'},
  //       { id: 4, name: "Monica Geller", phone: '714-541-3336', profession: 'Head Chef' },
  //       { id: 5, name: "Joey Tribbiani", phone: '972-297-6037', profession: 'Actor' },
  //       { id: 6, name: "Phoebe Buffay", phone: '760-318-8376', profession: 'Masseuse' }
  //     ]
  //   }
  // })
}
</script>
<style>
 
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
   padding-left: 250px;
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

 table {
  font-family: 'Open Sans', sans-serif;
  width: 750px;
  border-collapse: collapse;
  border: 3px solid #44475C;
  margin: -2px 15px 2px 20px;
}

table th {
  text-transform: uppercase;
  text-align: left;
  background: #44475C;
  color: #FFF;
  padding: 8px;
  min-width: 30px;
}

table td {
  text-align: left;
  padding: 8px;
  border-right: 2px solid #7D82A8;
}
table td:last-child {
  border-right: none;
}
table tbody tr:nth-child(2n) td {
  background: #D4D8F9;
}

 @media screen and (max-width: 780px) {
   .title-3  {  
    margin-right: 100px;
   }
   .lists-3 {
     padding-left: 105px;
   }
   .table {
     /* padding-right:  200px; */
   }
 }
</style>