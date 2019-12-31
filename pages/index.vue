<template>
       <div class="container">
  
         <img　class="pc" src="/white-cloud.jpeg">
         <img class="sp" src="/hand.jpeg" alt="スマホ用背景">


       </div>
</template>

<style scoped>
.container{
   margin-top:100px;
   text-align:center;
  
    } 
.container img{

  max-width: 100%; 

}
.pc { display: block !important; }
.sp { display: none !important; }

@media only screen and (max-width: 768px){
  .container{
   margin-top:10px;
   text-align:center;
  
    } 
    
    .pc { display: none !important; }
    .sp { display: block !important; }
}


  
</style>