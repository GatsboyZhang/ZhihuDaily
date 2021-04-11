<template>
  <div id="app">
<<<<<<< Updated upstream
    <my-nav></my-nav>
    <my-header></my-header>
    <my-content></my-content>
    <my-more></my-more>
    <my-footer></my-footer>
=======
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
        <div class='content_box1' v-for="s in stories">
        <span>{{s.title}}</span>
        <img v-bind:src="s.images[0]" style="width:100%"></img>
        </div>
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
>>>>>>> Stashed changes
  </div>
</template>

<script>

import MyNav from './components/MyNav.vue'
import MyHeader from './components/MyHeader.vue'
import MyContent from './components/MyContent.vue'
import MyMore from './components/MyMore.vue'
import MyFooter from './components/MyFooter.vue'
export default {
  name: 'App',
<<<<<<< Updated upstream
  components: {
    MyNav,
    MyHeader,
    MyContent,
    MyMore,
    MyFooter
=======
  data: () => {
  return {
    stories: []
    }
  },
  methods: {
    created: function(){
      console.log('1111111')
    }
  },
  mounted: function(){
      const that = this
      fetch('/zhihu/api/4/news/latest', {
      method: 'GET',
      headers: {'Access-Control-Allow-Origin': '*'}})
      .then((response) => {
        return response.json()
      })
      .then((json)=> {
      console.log(json.stories)
      that.$data.stories = json.stories
      })
>>>>>>> Stashed changes
  }
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

<<<<<<< Updated upstream
=======
  width: 100%;
  background-color: red;
  margin-bottom: 15px;
  padding-bottom: -10px
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
>>>>>>> Stashed changes
</style>