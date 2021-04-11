<template>
  <div id="app">
    <my-nav></my-nav>
    <my-header></my-header>
    <my-content></my-content>
    <my-more></my-more>
    <my-footer></my-footer>
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
  components: {
    MyNav,
    MyHeader,
    MyContent,
    MyMore,
    MyFooter
  },
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

</style>