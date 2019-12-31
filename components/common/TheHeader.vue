<template>
    

  
 

      <header class="header">
        <div class="main_navigation">
            <router-link to="/">
                <img src="@/assets/images/konamiota.JPG" alt="home">
            </router-link>
        </div>
         <div class="sns_navigation">
            <ul>
                <li><span><a href="https://www.facebook.com/konami.ota.73" target="_blank">
                <img src="@/assets/icons/FB_icon.png" alt="fb" >
                </a></span></li>
                <li><span><a href="https://www.instagram.com/kona_pasyo/" target="_blank">
                <img src="@/assets/icons/INSTAGRAM.png" alt="insta" >
                </a></span></li>
                <li><span><a href="https://twitter.com/kona_peso" target="_blank">
                <img src="@/assets/icons/TWITTER.png" alt="twi" >
                </a></span></li>
            </ul>
         </div>
    
        </header>

    
</template> 

<style scoped>
    .header{
    z-index: 20;
    position: fixed;
    top: 0px;
    width: 100%;
    height: 90px;
    background-color:#fff;

  box-shadow: 0px 6px 3px -3px rgba(0,0,0,0.05);
  -webkit-box-shadow: 0px 6px 3px -3px rgba(0,0,0,0.05);
  -moz-box-shadow: 0px 6px 3px -3px rgba(0,0,0,0.6);


    }
    .main_navigation {
    font-weight: bold;
    margin-left: auto;
    margin-right: auto;
    max-width: 630px;
    text-align: center;
    }
    .main_navigation img {
        width:100%;
        max-width: 300px;
        height: auto;
        margin-top:20px;

    }
 
    .sns_navigation {
    position: fixed;
    right: 60px;
    top: 40px;
    max-width: 202px;
 }
    

    .sns_navigation ul {
    height: 10px;
    display: inline-block;
    
}
    .sns_navigation li{
    list-style: none;
    float:left;

    }
    .sns_navigation img{
        height: 20px;
        width:20px;
        margin-right: 20px;
    }

    @media only screen and (max-width: 600px){
    .header{
        height:50px;
    }
    .main_navigation {
    width: 170px;
    float:left;
    margin-left:1em;
     margin-top:-5px; 
    }
    .main-navigation img{
        width:200px;
        height: auto;   
       
    }
    .sns_navigation{
        right: 0px;
        top:10px ;
    }
    .sns_navigation img{
        height: 15px;
        width:auto;
        margin-right: 20px;
    }
}
    

</style>
