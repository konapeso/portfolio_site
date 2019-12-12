<template>
    <header id="header">
        <nav id="main_navigation"><nuxt-link to="/"><img src="@assets/images/konamiota.jpg"></nav>
        <nav id="sns_navigation">
            <ul>
                <li><span><a href="https://www.facebook.com/konami.ota.73">
                <img src="@/assets/icons/FB_icon.png" alt="" height="15px" width="15px">
                </a></span></li>
                <li><span><a href="https://www.instagram.com/kona_pasyo/">
                <img src="@/assets/icons/INSTAGRAM.png" alt="" height="15px" width="15px">
                </a></span></li>
                <li><span><a href="https://www.instagram.com/kona_pasyo/">
                <img src="@/assets/icons/TWITTER.png" alt="" height="15px" width="15px">
                </a></span></li>
            </ul>
        </nav>
    </header>
</template> 

<style>
    #header{
   z-index: 20;
    position: fixed;
    top: 0px;
    width: 100%;
    height: 90px;
    background-color:#fff;

    }
    #main_navigation {
    font-weight: bold;
    margin-left: auto;
    margin-right: auto;
    width: 630px;
    text-align: center;
}
 
    #sns_navigation {
    position: fixed;
    right: 60px;
    top: 40px;
    width: 202px;
 }
    #nav ul{
        list-style: none;
    }

    #nav li {
    height: 10px;
    display: inline-block;
}

    

</style>
