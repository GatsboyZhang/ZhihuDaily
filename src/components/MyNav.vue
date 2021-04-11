<template>
    <div class='nav'>
      <div class='inner'>
        <div class='logo'></div>
        <a href='#' class='logo_content'>浏览内容</a>
        <a href='#' class='download'>App 下载</a>
      </div>
    </div>
</template>

<script>

export default {
  name: 'MyNav',
  data () {
    return {
      msg: 'MyNav'
    }
  }
}
</script>

<style scoped>
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
  background-image: url(../assets/logo.png);
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
</style>
