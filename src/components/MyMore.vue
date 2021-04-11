<template>
    <div class='more'>更多精彩内容可以在知乎日报中查看</div>
</template>

<script>

export default{
    name:'MyMore',
    data(){
        return {
            msg:'MyMore'
        }
    }
}
</script>

<style scoped>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
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
