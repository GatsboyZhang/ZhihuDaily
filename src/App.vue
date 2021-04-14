<template>
  <div id="app">
    <my-nav></my-nav>
    <my-header></my-header>
      <my-content-nav></my-content-nav>
      <div class='blank'>
        <my-card id='stream' v-bind:url ="story.url" v-bind:title="story.title" v-bind:img-link="story.images[0]" v-for="story in stories"></my-card>
        <div></div>
      </div>
      <my-more @click="handle"></my-more>
    <my-footer></my-footer>
  </div>
</template>

<script>

import MyNav from './components/MyNav.vue'
import MyHeader from './components/MyHeader.vue'
import MyContentNav from './components/MyContentNav.vue'
import MyCard from './components/MyCard.vue'
import MyMore from './components/MyMore.vue'
import MyFooter from './components/MyFooter.vue'
export default {
  name: 'App',
  components: {
    MyNav,
    MyHeader,
    MyContentNav,
    MyCard,
    MyMore,
    MyFooter
  },
  data: () => {
  return {
    stories: [],
    url:'https://www.baidu.com'
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
      const array = []
      that.$data.stories = array.concat(json.stories).concat(json.stories).concat(json.stories)
      })
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
my-content-nav{
  position: relative;
  top:50px;
}
.blank{
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content:center;
  background-color: rgb(249, 249, 249);
  padding-left: 100px;
  padding-right: 100px;
}
#stream{
  display: inline-block;
}
#stream:hover{
  display: inline-block;
  background-color: red;
}
</style>