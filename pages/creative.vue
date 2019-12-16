<template>
 
      <v-container>

        
    
    
    <v-content class="my-5">
        <h3 class="ma-6">WEB SITE</h3>
      <v-layout row wrap>
        
        <v-flex xs12 sm6 md4 lg3 v-for="(repo, i) in repos" :key="i">
          <a :href="repo.link" target="_blank">
            <v-hover
                  v-slot:default="{ hover }"
                  :open-delay="hover.openDelay"
                  :close-delay="hover.closeDelay"
                  :disabled="hover.disabled"
                  :value="hover.value"
                >
          <v-card :elevation="hover ? 8 : 2" class=" text-xs-center ma-3">
            <v-img :src="repo.image" height="300px" >
            </v-img>
            <v-card-text>
              <div class="subheading">{{ repo.name }}</div>
              <div class="gray--text">{{ repo.lang }}</div>
            </v-card-text>
            
          </v-card></v-hover>
          </a>
        </v-flex>
      </v-layout>
    
    </v-content>
    <v-content>
        <h3 class="ma-8">Works</h3>
        <v-row>
          
            <v-col cols="6" sm="4" v-for=" (work, i) in works" :key="i">
            <v-img :src="work.img"></v-img>
            </v-col>
        
        </v-row>
    </v-content>

    <h3 class="mt-10">illustration</h3>
    <v-row>
        
      <v-col cols="12" sm="6" offset-sm="3">
       

        <v-card class="mt-4 mb-4">
            <v-layout row wrap>
                <v-flex xs4 v-for="(item,i) in items" :key="i">
                <v-card>
                    <v-card-text>
                        <img v-bind:src="item.src" width="100%" alt="">
                    </v-card-text>
                </v-card>
                </v-flex>
            </v-layout>
        </v-card>
  
     
      </v-col>
    </v-row>
</v-container>
</template>

<style scoped>
.container {
  padding: 90px 50px 60px 50px;
  height: 100%;
  text-align: center;
}


a {
text-decoration: none;
}

a:visited {
  color : ＃808080; 
}
</style>

<script>
import GitHubImage from "@/assets/images/GitHub.png";

export default {
  data() {
    return {
      hover: [
        {
          disabled: false,
          openDelay: "0",
          closeDelay: "0",
          value: false
        }],
      repos: [
        { name: "イベントサイト", lang:"HTML/CSS", image:'/zeleplus.png', link:"https://zeleplus.com"},
        { name: "プロフィールサイト", lang:"HTML/CSS", image:'/page4.JPG', link:"https://jovial-cori-516369.netlify.com/profile.html"},
        { name: "Qiitaリアルタームサーチ", lang: "Vue.js", image: '/page3.png', link:"https://objective-euler-6be823.netlify.com/" },
        { name: "チャットアプリ", lang: "Vue.js/Firebase", image: '/page1.png', link:"https://stupefied-dubinsky-d35a10.netlify.com/#/"},
        { name: "ブログアプリ", lang: "Nuxt.js/Firebase", image: GitHubImage, link:"https://github.com/konapeso/nuxt-blog-service" },
        { name: "タイピングゲーム", lang: "JavaScript", image: '/page2.png', link:"https://affectionate-austin-857211.netlify.com/sample.html" },
       
      ],
      works:[
          { img: require("../assets/works/works1.JPG")},
          { img: require("../assets/works/works2.jpg")},
          { img: require("../assets/works/work4.jpg")}
      ],
      items: [
                {src: '/illust1.JPG'},
                {src: '/illust2.JPG'},
                {src: '/illust3.JPG'},
                {src: '/illust4.JPG'},
                {src: '/illust5.JPG'},
                {src: '/logo1.JPG'}
            
            ]
      
     
    };
  }
};
</script>