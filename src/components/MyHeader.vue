<template>
    <div class='header'>
      <div class='phone_sample'></div>
      <div class='new'>   
        <h1>每天三次，每次七分钟</h1>
        <p>在中国，咨询类移动应用的人均阅读时长是5分钟，而在知乎日报，这个数字是21。</p>
      </div>
      <div class='erweima'>
        <img src="../assets/qr_top2.png" class='header_img'>
      </div>
      <div class='ios'>
        <img src="../assets/iphone_logo.png" class='header_img'>
        <h4 class='ios_text'>iOS版</h4>
      </div>
      <div class='android'>
        <img src="../assets/android_logo.png" class='header_img'> 
        <h4 class='android_text'>Android版</h4>
      </div>
    </div>
</template>

<script>
export default{
    name: 'MyHeader',
    data() {
        return {
            msg:"MyHeader"
        }
    }
}
</script>

<style scoped>
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
  background-image: url(../assets/phone_sample.png);
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
</style>