<template>
  <div>
    <header>
      <p class="p2">首页</p>
      <div class="titlee">
      <img src="../../assets/images/drawable-xxhdpi-v4/sa.png" style="width: 2.7rem;">
      <img src="../../assets/images/drawable-xxhdpi-v4/ccc.png" style="width: 2.7rem;">
      <img src="../../assets/images/drawable-xxhdpi-v4/zzz.png" style="width: 2.7rem;">
      </div>
    </header>
    <div class="page-content" id="page-content">
      <m-swipe swipeid="swipe01" :autoplay="3000" paginationDirection="right">
        <div class="swiper-slide " slot="swiper-con"><img src="../../assets/images/drawable-xxhdpi-v4/123.png" alt=""></div>
        <div class="swiper-slide " slot="swiper-con"><img src="../../assets/images/drawable-xxhdpi-v4/234.jpg" alt=""></div>
        <div class="swiper-slide " slot="swiper-con"><img src="../../assets/images/drawable-xxhdpi-v4/342.jpg" alt=""></div>
      </m-swipe>
      <div class="var" >
        <div class="varse">
          <img src="../../assets/images/ic_camera_white.png"  >
          <p >发现</p>
        </div>
        <div class="varse">
          <img src="../../assets/images/ic_camera_white.png"  >
          <p >发现</p>
        </div>
        <div class="varse">
          <img src="../../assets/images/ic_camera_white.png" >
          <p >发现</p>
        </div>
        <div class="varse">
          <img src="../../assets/images/ic_camera_white.png"  >
          <p >发现</p>
        </div>
        <div class="varse">
          <img src="../../assets/images/ic_camera_white.png"  >
          <p >发现</p>
        </div>
      </div>
      
      <!--热门-->
      <div class="hot-wrap">
        <div class="titl">
          <span>
            <img src="../../assets/images/drawable-xxhdpi-v4/icon_recommend_course.png" alt="">课程推荐
          </span>
          <a href="javascript:;">换一换</a>
        </div>

        <div class="contents">
          <p class="tit-l">java</p>
          <div class="cont">
            <h6>java消息中间件</h6>
            <p >使用java消息中间件处理一部消息</p>
            <p>1360人学习</p>
          </div>
        </div>
        <div class="contents">
          <p class="tit-l">java</p>
          <div class="cont">
            <h6>java消息中间件</h6>
            <p >使用java消息中间件处理一部消息</p>
            <p>1360人学习</p>
          </div>
        </div>
        <div class="contents">
          <p class="tit-l">java</p>
          <div class="cont">
            <h6>java消息中间件</h6>
            <p >使用java消息中间件处理一部消息</p>
            <p>1360人学习</p>
          </div>
        </div>
        <div class="contents">
          <p class="tit-l">java</p>
          <div class="cont">
            <h6>java消息中间件</h6>
            <p >使用java消息中间件处理一部消息</p>
            <p>1360人学习</p>
          </div>
        </div>
       <div style="clear: both;"> </div>
      </div>

      <div class="urls">
        <div class="titl">
          <span>
            <img src="../../assets/images/drawable-xxhdpi-v4/share_icon.png" alt="">职业路径
          </span>
          <a href="javascript:;">换一换</a>
        </div>
        <div class="tones">
            <div class="imgs">
              HTML/CSS <br>
              javascript <br>
              jQuery
            </div>
            <div class="tret">
              <h5>前端小白入门</h5>
              <p class="texts">从小白到老司机，学会HTML，CSS，JS，jQuery基础，独立开发挂号平台网页</p>
              <p class="texte">33门可/12124人学习<span>&nbsp;&nbsp;&nbsp;￥499.00</span></p>
            </div>
          </div>
        <div class="tones">
            <div class="imgs">
              HTML/CSS <br>
              javascript <br>
              jQuery
            </div>
            <div class="tret">
              <h5>前端小白入门</h5>
              <p class="texts">从小白到老司机，学会HTML，CSS，JS，jQuery基础，独立开发挂号平台网页</p>
              <p class="texte">33门可/12124人学习<span>&nbsp;&nbsp;&nbsp;￥499.00</span></p>
            </div>
          </div>
        <div class="tones">
            <div class="imgs">
              HTML/CSS <br>
              javascript <br>
              jQuery
            </div>
            <div class="tret">
              <h5>前端小白入门</h5>
              <p class="texts">从小白到老司机，学会HTML，CSS，JS，jQuery基础，独立开发挂号平台网页</p>
              <p class="texte">33门可/12124人学习<span>&nbsp;&nbsp;&nbsp;￥499.00</span></p>
            </div>
          </div>
      </div>
      <!--推荐-->
      <!--<div class="recommend-wrap">
        <m-cell title="推荐" label="recommend"></m-cell>
        <m-cell-media  :author="item.target.author.name" :column="item.source_cn" :bg="item.target.cover_url" v-for="(item,index) in recommendData" :key="item.id">
          <span slot="title">{{item.title}}</span>
          <span slot="describe">{{item.target.desc}}</span>
        </m-cell-media>
      </div>-->
      <div><br><br><br><br><br><br></div>
    </div>
  </div>
</template>

<script>
  import mHeader from '../../components/header'
  import mSwipe from '../../components/swipe'
  import mCell from '../../components/cell'
  import mCellMedia from '../../components/cell-media'
  export default {
    name: 'index',
    components: {
      mHeader,
      mSwipe,
      mCell,
      mCellMedia
    },
    data() {
      return {
        recommendData: [],
        hotData: []
      }
    },

    created() {
      this.fetchData();
    },
    methods: {
      /*fetchData() {
        this.axios.get('/api/homeData').then((response) => {
          let data = response.data.data.recommend_feeds;
          let recommend = [];
          let hot = [];
          for (var i in data) {
            if (data[i].card && data[i].card.name == '为你推荐') {
              recommend.push(data[i]);
            } else {
              hot.push(data[i]);
            }
          }

          this.recommendData = recommend;
          this.hotData = hot;

        })
      }*/
    }
  }

</script>

<style lang="less">
  #page-content{
    height: 12rem;
  }
  .is-fixed~.page-content {
    padding-top: 2rem;
    padding-bottom: 2ewm;
    
  }
  .page-content {
    .var{
      .varse{
        float: left;
        margin: 2% 5.2% 2% ;
        img{
          width:1.5rem;
        }
        p{
          font-size: .5rem; 
          text-align: center;
           padding-top: .1rem;
            color: #000;
        }
      }
    }
  }
  .top-search {
    .p1 {margin-right: 22rem;}
    
    .search-wrap {
      float:right;
      .placeholder {
        
        text-align: left;
        padding-left: 12px;
      }
      img {
        float: left;
        width: 20px;
        height: 20px;
        display: inline-block;
      }
    }
  }
  .hot-wrap{
    clear: both;
    background: #EEE;
    padding-bottom:2rem;
  }
  .hot-wrap,
  .recommend-wrap {
    padding-top: 1rem;
  }
  .titl{
    text-align: center;
    span{
      padding-left: 3rem;
      font-family: 楷体;
      font-size: .8rem;
        img{
        width: 1rem;
        height: 1rem;
        margin-right: .5rem;
      }
    }
    a{
      font-family: 楷体;
      font-size: .5rem;
      color: #000;
      float: right;
      margin: .3rem .9rem 0 0;
    }
  }
  .contents{
    float: left;
    width: 7.3rem;
    height: 6rem;
    font-family: 楷体;
    margin: 1.1rem 0 0 .4rem;
    border-radius: 3px;
    border: 1px solid #FFF;
    background: #FFF;
      line-height: 1rem;
    box-shadow: .2rem .2rem .2rem #999;
    .tit-l{
      height: 1.3rem;
      width: 7.3rem;
      font-size: .6rem;
      color: #fff;
      padding-top:.1rem;
      text-indent: .6rem;
      background:url("../../assets/images/drawable-xxhdpi-v4/21a948ea42dd89ea6e3d1e25ff131cd2.jpg");
      border-radius:3px;
    }
    .cont{
      padding: .2rem .2rem 0 .6rem;
    }
    &:before{

    cleat: both;
    }

  }
  .urls{
      padding: 1rem;
      .tones{
          padding: .5rem 0 1rem 0;
          clear: both;
        .imgs{
          float: left;
          padding: .5rem 0 0 .6rem;
          width: 4rem;
          height:3.7rem;
          color: #fff;
          font: .2rem 楷体;
          background: url("../../assets/images/9612b3a2fcd8d73446c8858a60168808.jpg") ;
          background-size: 5rem 5rem;
        }
        .tret{
          font-family: 楷体;
          padding:.1rem 0 0 4.5rem;
          h5{
            font-size: .7rem ;
          }
          .texts{
            color: #aaa;
            font-size: .3rem;
          }
          .texte{
            padding-top: .3rem;
            font-size: .3rem;
            color: #222;
            span{
              color: red;
            }
          }
        }
      }
    }
</style>
