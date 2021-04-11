<template>
    <div class='footer'>
        <div class='text_box'>
            &nbsp;
            <p>知乎日报是一款拥有千万用户的资讯类客户端，每日提供来自知乎社区的精选问答，还有国内一流媒体的专栏特稿。</p>
            &nbsp;
            <p>主题日报包括动漫、设计、大公司、游戏、财经、电影、电子音乐、互联网安全等丰富内容，为业内人和资深爱好者推荐各领域最精彩文章，满足高质量阅读需求。</p>
            &nbsp;
            <p>在知乎日报，告别浮躁，重获阅读的愉悦。</p>
            &nbsp;
            <p id='police_side'>京 ICP 证 110745 号</p>
            &nbsp;
            <img src="../assets/police.png" id='police'>
            <p>京公网安备 11010802010035 号</p>
            &nbsp;
            <p>©zhihu 2015</p>
        </div>
        <div class='erweima'>
            <img src="../assets/qr_top2.png" class='header_img'>
        </div>
        <p id='last_text'>扫描客服端下载</p>
    </div>
</template>

<script>

export default{
    name:'MyFooter',
    data() {
        return {
            msg:"MyFooter"
        }
    }
}
</script>

<style  scoped>
.footer{
    width:100%;
    height: 320px;
    margin-top: 30px;
    background-color: #e5e5e5;
}
.footer .text_box{
    display: inline-block;
    width: 50%;
    margin-left:16.5%;

}
.footer .text_box #police{
    position: relative;
    bottom: 22px;
    right:12px;
}
.footer .text_box #police_side{
    position: relative;
    left:22px;
}
.footer p{
    font-size: 14px;
    line-height: 26px;
    color: #666
}
.footer .erweima{
  float: right;
  position: relative;
  width: 145px;
  height: 153px;
  right:238px;
  top:25px;
  background-color: white;
  border-radius: 5px;
}
.header_img{
  display: inline-block;
  padding-left: 5px;
  padding-top:9px;
}
#last_text{
    position: relative;
    float: right;
    font-size: 18px;
    top:200px;
    right:100px;
}
</style>