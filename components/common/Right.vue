<template>
    <div id="right">
        <nav id="right_navigation">
            <ul>    
                <li>
                    <router-link to="/contact">
                        <span>CONTACT</span>
                    </router-link>
                </li>
                <li>
                    <router-link to="/activity">
                        <span>ACTIVITY</span>
                    </router-link>
                </li>
            </ul>

        </nav>
    </div>
</template>

<style>

#right {
    z-index: 5;
    position: fixed;
    right: 0px;
    top: 90px;
    bottom: 60px;
    width: 60px;
}

#right_navigation{
    position: fixed;
    right: 0px;
    bottom: 100px;
    height: 200px;
    margin-right: -100px;
    
}

#right_navigation ul{

    list-style:none;
    display: inline-block;
    transform: rotate(90deg);
}



#right #right_navigation ul li {
    margin-left: 80px;
    height: 18px;
    display: inline-block;
}


</style>