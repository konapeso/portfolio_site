<template>
    
        <v-flex xs6 md6>
  
 

      <header id="header">
        <nav id="main_navigation">
            <router-link to="/">
                <img src="@/assets/images/konamiota.JPG" alt="home">
            </router-link>
            </nav>
         <nav id="sns_navigation">
            <ul>
                <li><span><a href="https://www.facebook.com/konami.ota.73">
                <img src="@/assets/icons/FB_icon.png" alt="fb" >
                </a></span></li>
                <li><span><a href="https://www.instagram.com/kona_pasyo/">
                <img src="@/assets/icons/INSTAGRAM.png" alt="insta" >
                </a></span></li>
                <li><span><a href="https://www.instagram.com/kona_pasyo/">
                <img src="@/assets/icons/TWITTER.png" alt="twi" >
                </a></span></li>
            </ul>
         </nav>
        </header>
     </v-flex>
    
</template> 

<style scoped>
    #header{
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
    #main_navigation {
    font-weight: bold;
    margin-left: auto;
    margin-right: auto;
    width: 630px;
    text-align: center;
}
    #main_navigation img {
        width: 300px;
        margin-top:20px;

    }
 
    #sns_navigation {
    position: fixed;
    right: 60px;
    top: 40px;
    width: 202px;
 }
    

    #sns_navigation ul {
    height: 10px;
    display: inline-block;
    
}
    #sns_navigation li{
    list-style: none;
    float:left;

    }
    #sns_navigation img{
        height: 20px;
        width:20px;
        margin-right: 20px;
    }
    

</style>
