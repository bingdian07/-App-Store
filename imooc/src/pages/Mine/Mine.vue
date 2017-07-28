<template>
  <div class="apps">
    <header>
      <p class="p2">我的</p>
      <div class="titlee">
      <img src="../../assets/images/drawable-xxhdpi-v4/sa.png" style="width: 2.7rem;">
      <img src="../../assets/images/drawable-xxhdpi-v4/ccc.png" style="width: 2.7rem;">
      <img src="../../assets/images/drawable-xxhdpi-v4/zzz.png" style="width: 2.7rem;">
      </div>
    </header>
    <div class="vars">
      <div class="tops">
      <div style="clear: both;"></div>
        <p class="head-img"><img src="../../assets/images/drawable-xxhdpi-v4/f009.png"></p>
        <div class="img-right">
          <h5>冰点5</h5>
          <p class="p3">学习时长<span>4小时</span>&nbsp;&nbsp;|<span>经验&nbsp;&nbsp;90</span></p>
        </div>
      </div>
      <div class="bottoms">
        <p>关注  1<p>|</p></p>
        <p>粉丝  1<p>|</p></p>
        <p>积分  1</p>
      </div>
    </div>
    <div class="carte">
      <div class="cartes">
        <img src="../../assets/images/ic_my_note.png" >
        <p>我的课程</p>
      </div>
      <div class="cartes">
        <img src="../../assets/images/ic_my_note.png" >
        <p>我的课程</p>
      </div>
      <div class="cartes">
        <img src="../../assets/images/ic_my_note.png" >
        <p>我的课程</p>
      </div>
      <div class="cartes">
        <img src="../../assets/images/ic_my_note.png">
        <p>我的课程</p>
      </div>
    </div>
    
      <div class="lists">
        <div class="ones">
          <img src="../../assets/images/drawable-xxhdpi-v4/teacher_icon.png" >
          <span>历史记录</span>
          <img class="ones-img" src="../../assets/images/drawable-xxhdpi-v4/download_complete_icon.png">
        </div>
        <div class="ones">
          <img src="../../assets/images/drawable-xxhdpi-v4/teacher_icon.png" >
          <span>历史记录</span>
          <img class="ones-img" src="../../assets/images/drawable-xxhdpi-v4/download_complete_icon.png" >
        </div>
        <div class="ones">
          <img src="../../assets/images/drawable-xxhdpi-v4/teacher_icon.png" >
          <span>历史记录</span>
          <img class="ones-img" src="../../assets/images/drawable-xxhdpi-v4/download_complete_icon.png" >
        </div>
      </div>

      <div class="lists">
        <div class="ones">
          <img src="../../assets/images/drawable-xxhdpi-v4/teacher_icon.png" >
          <span>历史记录</span>
          <img class="ones-img" src="../../assets/images/drawable-xxhdpi-v4/download_complete_icon.png" >
        </div>
        <div class="ones">
          <img src="../../assets/images/drawable-xxhdpi-v4/teacher_icon.png" >
          <span>历史记录</span>
          <img class="ones-img" src="../../assets/images/drawable-xxhdpi-v4/download_complete_icon.png" >
        </div>
        <div class="ones">
          <img src="../../assets/images/drawable-xxhdpi-v4/teacher_icon.png" >
          <span>历史记录</span>
          <img class="ones-img" src="../../assets/images/drawable-xxhdpi-v4/download_complete_icon.png" >
        </div>
      </div>

      <div class="lists">
        <div class="ones">
          <img src="../../assets/images/drawable-xxhdpi-v4/teacher_icon.png" >
          <span>历史记录</span>
          <img class="ones-img" src="../../assets/images/drawable-xxhdpi-v4/download_complete_icon.png" >
        </div>
        <div class="ones">
          <img src="../../assets/images/drawable-xxhdpi-v4/teacher_icon.png" >
          <span>历史记录</span>
          <img class="ones-img" src="../../assets/images/drawable-xxhdpi-v4/download_complete_icon.png" >
        </div>
      </div>
    
 <span>icon 是图片</span>
  </div>
</template>

<script>
  import mHeader from '../../components/header'
  export default {
    name: 'mine',
    components: {
      mHeader
    }
  }
</script>


<style lang="less">
.apps{
  background:#eee;
}
header{
  background: #444;
  color: #fff;
  font-family: 楷体;
  clear:both;
  padding: .4rem .8rem 1.3rem;
  .p2{
      float: left;
      font-size: .5rem;
  }
  .titlee{
    float: right;
    img{padding-left: 1.7rem;}

  }
}
.vars{
  background: #fff;
    padding: 1rem;
  .tops{
    height: 3.4rem;

    .head-img{
      float: left;
      width: 3rem;
      height: 3rem;
      overflow: hidden;
      border-radius: 50%;
      border: 1px solid;
      position: relative;
      img{
        position: absolute;
        left: .1rem;
        top: .2rem;
        wdith:2.8rem;
        height:2.8rem;
      }
    }
    .img-right{
      float: left;
      padding: .3rem 0 0 .5rem;
      h5{
        font: .8rem 楷体;
        padding: 0 0 .3rem 0;
      }
      .p3{
        font: .5rem 楷体;
        span{
          padding-left: 1rem;
        }
      }
    }

  }
  .bottoms{
      p{
        float: left;
        margin-left: 1.6rem;
        font-size: .4rem;
      }
    }
}
.carte{
      margin-top: .6rem;
      padding: 1rem 0;
      background: #fff;
      height: 4rem;
      .cartes{
        float: left;
        padding-left:  1.27rem;
        img{
          margin-left: .4rem;
          width:1.8rem
        }
        font-size: .6rem;
        font-family: 楷体;
      }
    }
    .lists{
      height: 6.7rem;
      margin: .5rem 0;
      background: #fff;
      .ones{
        padding: .5rem 1rem;
        span{
          margin-left: 1rem;
          font:.9rem 楷体;
        }
        img{
          width: 1.1rem;
        }
        .ones-img{
          float: right;
        }
      }
    }
</style>