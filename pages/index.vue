<template>
       <div class="container">
  
         <img　class="pc" src="/white-cloud.jpeg">
         <img class="sp" src="/hand.jpeg" alt="スマホ用背景">


       </div>
</template>

<style scoped>
.container{
   margin: 0 auto;
   text-align:center;
  
    } 
.container img{
  max-width: 100%; 
  height: 600px;
  margin-top:70px;

}
.sp { display: none; }

@media only screen and (max-width: 768px){
  .container{
   margin-top:80px;
   text-align:center;
  
    } 
    .container img{
      width: 250px; 
      height: 100%;
      margin-top:0 ;

}
    .pc { display: none; }
    .sp { display: inline ; }
}


  
</style>