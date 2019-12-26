<template>
    
<v-container class="mt-5">
   <h1>CONTACT ME &nbsp;</h1>
   <br><br>

    <form action="" method="post">
        <div class="item">
        <label class="label" for="yourname">お名前</label> 
        
        <input id="rendou" type="text" name="yourname" placeholder="your name"></div>
        <div class="item">
        <label class="label">メールアドレス</label>
        <input class="inputs" type="email" name="email">
        </div>
        <div class="item">
        <label class="label" for="comment">コメント</label>
        <textarea id="comment" name="comment" placeholder="ご自由に入力ください"></textarea>
        </div>
        <input type="submit" value="送信する">
 
        
    </form>
</v-container>
</template>

<style scoped>
form{
  width:460px;
  margin:0 auto;
}
.item{
  overflow: hidden;
  margin-bottom: 20px;
}
.label{
  float: left;
  margin-right: 20px;
  width:135px;
  border-left: solid 3px #e0505d;
  padding-left: 10px;
}
.inputs{
  float: left;
  width:300px;
}
input[type="text"],input[type="email"]{
  border: solid 1px #aaa;
  border-radius:5px;
  padding:10px;
  font-size: 15px;
}
textarea{
  border: solid 1px #aaa;
  border-radius:5px;
  padding: 10px;
  height: 160px;
  font-size: 15px;
}
input[type="submit"]{
  background: #e0505c;
  border: none;
  color: white;
  font-size:17px;
  font-weight:bold;
  padding: 10px 20px;
  margin: 0 5px;
}


</style>