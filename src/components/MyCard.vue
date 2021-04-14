<template>
    <div class='card' @click="handle">
        <img v-bind:src="imgLink" class='content'>
        <span>{{title}}</span>
        <span>{{clickCount}}</span>
    </div>
</template>

<script>

export default{
    name:'MyCard',
    props: {
        title: '',
        imgLink: '',
        url: ''
    },
    data(){
        return{
            msg:'MyCard',
            clickCount: 0
        }
    },
    methods: {
        handle: function(){
            window.open(this.$props.url)
            this.$data.clickCount = this.$data.clickCount+1
        }
    },
    created: function() {
        console.log(this.$props)
    }
}
</script>

<style scoped>
.card{
    position: relative;
    width:320px;
    border-radius: 5px;
    margin: 20px;
    background-color: #fff;
}
.card .content{
    font-size: 22px;
    color: #000;
    line-height: 30px;
}
img{
    z-index: 100;
    width:280px;
    padding-top:20px;
    padding-left:20px;
}
span{
    display: inline-block;
    position: relative;
    width: 80%;
    margin-top: 20px;
    margin-left: 5%;
    margin-bottom:20px ;
}

</style>