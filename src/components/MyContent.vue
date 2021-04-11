<template>
       <div class='content'>
      <div class='content_nav'>
        <span class='through'>浏览内容</span>
        <span class='new_content'>最新内容</span>
      </div>
      <div class='stream1'>
        <div class='content_box1' v-for="item in 10">{{item}}</div>
      </div>
      <div class='stream2'>
        <div class='content_box2' v-for="item in 10">{{item}}</div>
      </div>
      <div class='stream3'>
        <div class='content_box3' v-for="item in 10">{{item}}</div>
      </div>
    </div>
</template>

<script>
export default{
    name:'MyContent',
    data() {
        return {
            msg:'MyContent'
        }
    }
}
</script>

<style scoped>
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
</style>
