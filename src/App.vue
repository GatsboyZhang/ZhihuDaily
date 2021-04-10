<template>
  <div id="app">
    <div class='nav'>
      <div class='inner'>
        <div class='logo'></div>
        <a href='#' class='logo_content'>浏览内容</a>
        <a href='#' class='download'>App 下载</a>
      </div>
    </div>
    <div class='header'>
      <div class='phone_sample'></div>
      <div class='new'>   
        <h1>每天三次，每次七分钟</h1>
        <p>在中国，咨询类移动应用的人均阅读时长是5分钟，而在知乎日报，这个数字是21。</p>
      </div>
      <div class='erweima'>
        <img src="./assets/qr_top2.png" class='header_img'>
      </div>
      <div class='ios'>
        <img src="./assets/iphone_logo.png" class='header_img'>
        <h4 class='ios_text'>iOS版</h4>
      </div>
      <div class='android'>
        <img src="./assets/android_logo.png" class='header_img'> 
        <h4 class='android_text'>Android版</h4>
      </div>
    </div>
    <div class='content'>
      <div class='content_nav'>
        <span class='through'>浏览内容</span>
        <span class='new_content'>最新内容</span>
      </div>
      <div class='stream1'>
        <div class='content_box1'></div>
        <div class='content_box1'></div>
        <div class='content_box1'></div>
        <div class='content_box1'></div>
        <div class='content_box1'></div>
        <div class='content_box1'></div>
        <div class='content_box1'></div>
        <div class='content_box1'></div>
        <div class='content_box1'></div>
        <div class='content_box1'></div>
      </div>
      <div class='stream2'>
        <div class='content_box2'></div>
        <div class='content_box2'></div>
        <div class='content_box2'></div>
        <div class='content_box2'></div>
        <div class='content_box2'></div>
        <div class='content_box2'></div>
        <div class='content_box2'></div>
        <div class='content_box2'></div>
        <div class='content_box2'></div>
        <div class='content_box2'></div>
      </div>
      <div class='stream3'>
        <div class='content_box3'></div>
        <div class='content_box3'></div>
        <div class='content_box3'></div>
        <div class='content_box3'></div>
        <div class='content_box3'></div>
        <div class='content_box3'></div>
        <div class='content_box3'></div>
        <div class='content_box3'></div>
        <div class='content_box3'></div>
        <div class='content_box3'></div>
      </div>
    </div>
    <div class='more'>更多精彩内容可以在知乎日报中查看</div>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
}
template {
    font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
.nav{
  background-repeat: no-repeat;
  width: 100%;
  height: 78px;
}
.nav .inner{
  width: 70%;
  height: 78px;
  margin-left: 15%;
}
.nav .logo{
  float: left;
  width: 172px;
  height: 78px;
  background-image: url(./assets/logo.png);
  background-size: 172px 78px;
}
.nav .logo_content{
  float: right;
  width: 132px;
  height: 32px;
  line-height: 78px;
  text-decoration: none;
  font-size:18px;
  color: black;
}
.nav .download{
  float: right;
  width: 132px;
  height: 32px;
  line-height: 78px;
  text-decoration: none;
  font-size: 18px;
  color: black;
}
.header{
  width: 100%;
  height: 460px;
  background-color:#008bed;
}
.header .phone_sample{
  display: inline-block;
  margin-left: 20%;
  margin-top:12px;
  width: 409px;
  height: 448px;
  background-image: url(./assets/phone_sample.png);
}
.header .new{
  margin-top:40px;
  float: right;
  margin-right: 18%;
  width: 402px;
  height: 150px;
}
.header h1{
  font-size: 40px;
  color: white;
}
.header p{
  color: #99d1f8;
  font-size: 16px;
  line-height: 26px;
  height: 100px;
}
.header .erweima{
  float: right;
  width: 145px;
  height: 153px;
  margin-top:-250px;
  margin-right: 510px;
  background-color: white;
  border-radius: 5px;
}
.header_img{
  display: inline-block;
  padding-left: 5px;
  padding-top:9px;
}
.header .ios{
  position: relative;
  float: right;
  width: 194px;
  height: 64px;
  margin-top:-250px;
  margin-right: 265px;
  background-color: white;
  border-radius: 3px;
}
.header .ios:hover{
  position: relative;
  float: right;
  width: 194px;
  height: 64px;
  margin-top:-250px;
  margin-right: 265px;
  background-color: #99d1f8;
  border-radius: 3px;
}
.header .android{
  position: relative;
  float: right;
  width: 194px;
  height: 64px;
  margin-top:-160px;
  margin-right: 265px;
  background-color: white;
  border-radius: 3px;
}
.header .android:hover{
  position: relative;
  float: right;
  width: 194px;
  height: 64px;
  margin-top:-160px;
  margin-right: 265px;
  background-color: #99d1f8;
  border-radius: 3px;
}
.header .ios_text{
  float: right;
  padding-right: 55px;
  padding-top: 18px;
  font-size: 24px;
  text-align: center;
  margin-bottom: 64px;
}
.header .android_text{
  float: left;
  z-index: 100;
  margin-left:57px;
  margin-top:-48px;
  font-size: 24px;
  text-align: center;
}
.content{
  width:100%;
  height: 3300px;
}
.content .content_nav{
  margin-top:50px;
  margin-left: 17%;
  width:65%;
  line-height: 50px;
  height: 50px;
}
.content .content_nav .through{
  font-size: 25px;
  color: #333333;
  line-height: 25px;
  height: 25px;
}
.content .content_nav .new_content{
  float: right;
  font-size: 25px;
  color: #CCCCCC;
  height: 25px;
}
.content .stream1{
  float: left;
  margin-left: 17%;
  height: 100%;
  width: 260px;
}
.stream1 .content_box1{

  width: 100%;
  height: 324px;
  background-color: yellow;
  margin-bottom: 15px;
}
.content .stream2{
  float: left;
  margin-left: 60px;
  height: 100%;
  width: 260px;
}
.stream2 .content_box2{
  width: 100%;
  height: 340px;
  background-color: yellow;
  margin-bottom: 15px;
}
.content .stream3{
  float: left;
  margin-left: 60px;
  height: 100%;
  width: 260px;
}
.stream3 .content_box3{
  width: 100%;
  height: 330px;
  background-color: yellow;
  margin-bottom: 15px;
}
.more{
  font-size: 20px;
  color: #15527b;
  background: #e8eef2;
  border-radius: 3px;
  display: block;
  text-align: center;
  height: 62px;
  width: 67%;
  margin-left: 16.5%;
  line-height: 62px;
  margin-top:300px
}
</style>