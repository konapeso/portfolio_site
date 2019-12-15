<template>
 
      <v-container>

        <v-content>
          <h3>WEB SITE</h3>
          <v-row align="center" justify="center">
          <v-card class="mx-auto" max-width="400" >
        <a href="http://zeleplus.com">
              <v-img class="white--text align-end" height="400px" src="/zeleplus.png">
                <v-card-title>zele+</v-card-title>
          
      </v-img></a>
      <v-card-text class="text--primary">
      <div>イベントサイト</div>

      <div>HTML/CSS</div>
    </v-card-text>
          </v-card>
          </v-row>
      </v-content>
    
    
    <v-content class="my-5">
        <h3>Git hub Repositories</h3>
      <v-layout row wrap>
        <v-flex xs12 sm6 md4 lg3 v-for="(repo, i) in repos" :key="i">
          <v-card class="text-xs-center ma-3">
            <v-img :src="repo.image" height="100px" >
            </v-img>
            <v-card-text>
              <div class="subheading">{{ repo.name }}</div>
              <div class="gray--text">{{ repo.role }}</div>
            </v-card-text>
            <v-card-actions>
              <div class="my-3">  
              <v-btn>
                <a :href="repo.link">GitHub</a>
              </v-btn>
              </div>
            </v-card-actions>
          </v-card>
        </v-flex>
      </v-layout>
    
    </v-content>
    <v-content>
        <h3>Works</h3>
        <v-row>
          
            <v-col cols="6" sm="4" v-for=" (work, i) in works" :key="i">
            <v-img :src="work.img"></v-img>
            </v-col>
        
        </v-row>
    </v-content>

    <h3>illustration</h3>
    <v-row>
        
      <v-col cols="12" sm="6" offset-sm="3">
       

        <v-card class="mt-4 mb-4 pa-3">
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

<style>
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
      repos: [
        { name: "Qiitaリアルタームサーチ", role: "Vue.js", image: GitHubImage, link:"https://github.com/konapeso/qiita_realtime_search" },
        { name: "チャットアプリ", role: "Vue.js/Firebase", image: GitHubImage, link:"https://github.com/konapeso/vue-firebase"},
        { name: "ブログアプリ", role: "Nuxt.js/Firebase", image: GitHubImage, link:"https://github.com/konapeso/nuxt-blog-service" },
        { name: "タイピングゲーム", role: "JavaScript", image: GitHubImage, link:"https://github.com/konapeso/typinggame_js" },
       
      ],
      works:[
          { img: require("../assets/works/works1.JPG")},
          { img: require("../assets/works/works2.jpg")},
          { img: require("../assets/works/works3.JPG")}
      ],
      items: [
                {src: '/illust1.JPG'},
                {src: '/illust2.JPG'},
                {src: '/illust3.JPG'},
                {src: '/illust4.JPG'},
                {src: '/illust5.JPG'}
            
            ]
      
     
    };
  }
};
</script>