<template>
    <div class='content'>
      <div class='content_nav'>
        <span class='through'>浏览内容</span>
        <span class='new_content'>最新内容</span>
      </div>
    </div>
</template>

<script>
export default{
    name:'MyContentNav',
    data() {
        return {
            msg:'MyContentNav'
        }
    }
}
</script>

<style scoped>
.content{
  width:100%;
}
.content .content_nav{
  margin-left: 17%;
  width:65%;
  margin-top:10px;
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
</style>
