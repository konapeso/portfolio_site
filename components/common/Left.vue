<template>
    <div id="left">
        <nav id="left_navigation">
            <ul>    
                <li>
                    <router-link to="/about">
                        <span>ABOUT</span>
                    </router-link>
                </li>
                <li>
                    <router-link to="/creative">
                        <span>CREATIVE</span>
                    </router-link>
                </li>
            </ul>

        </nav>
    </div>
</template>

<style scoped>
#left{
    z-index: 5;
    position: fixed;
    left: 0px;
    top: 90px;
    bottom: 100px;
    width: 60px;

    background-color: #fff;
}
#left_navigation{
    position: fixed;
    left: 0px;
    bottom: 100px;
    height: 200px;
   transform: rotate(-90deg);
}

#left_navigation ul{
  
    list-style:none;
}



#left #left_navigation ul li {
    margin-left: 80px;
    height: 18px;
    display: inline-block;
}

a:link,
a:visited,
a:hover,
a:active {
  color: #808080;
  text-decoration: none;
}

</style>