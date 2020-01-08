<template>
  <div class="main">
      <div class="main-container">
        <h2>ABOUT</h2>
        <div class=" main-profile">




          <div class ="profile-inner">
            <div class ="profile-image">
              <img src="/profile.jpg">
            </div>
            <div class="profile-detail">
              <div class="name-furigana" align="left">Konami Ota</div>
              <div class="wrap-name">
                <div class=" name-kanji">
                  <div class="kanji">大田　小波</div>
                  <ul class="sns">
                    <li><a class="fab fa-twitter twitter" href=" https://mobile.twitter.com/kona_peso">
                    </a></li>
                    <li><a class="fab fa-instagram instagram" href="https://www.instagram.com/kona_pasyo/"></a></li>
                  </ul>
                </div>
              </div>
              <div class="detail-text">
                <p>フロントエンドエンジニアを目指し奮闘中👩🏻‍💻</p>
                <p>CODE BASE 5期</p>
                <p>趣味でPOPやイラストを書いたり、小物を</p>
                <p>作ったり、いろんなことをしています。</p>
                <p>詳しくは、<router-link to="/activity">ACTIVITY</router-link>にて</p>
                
              </div>

            </div>
      </div>
  </div>
  </div>
  </div>
</template>

<style scoped>

.main{
  margin:90px 30px 30px 30px;

}
.main-container{
  padding:20px;

}
.main-container h2{
  text-align: center;
  margin:30px
}

.main-profile{

  margin: 0 280px;
  padding:0;
  box-sizing: border-box;

  border: 4px solid #f5f5f5;

}


.profile-inner{
  padding: 30px;
  display:flex;
  margin:0;

}

.profile-img{
  width: 350px;
  height: 350px;

  position:relative;

}
img{
  opacity:1;
  width: 350px;
  height: 350px;
  margin: 0;
  padding: 0;
}
.profile-detail{

  margin-left:30px;



}
.name-furigana {
  font-family: 'Dawning of a New Day', cursive;
  font-size: 25px;
  margin: 15px;
  color:#999;

}


.wrap-name{


  justify-content: space-between;
  margin-top:-20px;
  padding-top:0px;
  padding-bottom:30px;

}
.kanji{
  float:left;
  font-size:30px;
  font-family: 'Dawning of a New Day', cursive, 'M PLUS Rounded 1c', sans-serif;
  margin-top:-3px;
}

.name-kanji li{
  list-style: none;
  float:right;
  padding:0.5px;


  }

.twitter{
  color:gray;
  text-decoration:none;
  padding:2px;
  font-size:1.5em;

}

.instagram{
  color:gray;
  text-decoration:none;
  padding:2px;
  margin-right:2px;
  font-size: 1.5em;

}


  .detail-text{
    margin-top:30px ;

    float:left;
  }


  .detail-text li{

    list-style: none;
    text-align:left;
    float:left;
    font-size: 20px;
    padding:2px

  }
  .hashtag{
    margin-left: -30px;
    color:gray;

  }
  
</style>