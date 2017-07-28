<template>
  <div class="appes-list">
    <header>
      <p class="p2">课程</p>
      <div class="titlee">
        <img src="../../assets/images/drawable-xxhdpi-v4/sa.png" style="width: 2.7rem;">
        <img src="../../assets/images/drawable-xxhdpi-v4/ccc.png" style="width: 2.7rem;">
        <img src="../../assets/images/drawable-xxhdpi-v4/zzz.png" style="width: 2.7rem;">
      </div>
    </header>
    <div class="web-list">
    <h5>前端课程</h5>
      <div class="course">
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
      </div>
    </div>
    <div class="web-list">
    <h5>后端开发</h5>
      <div class="course">
        
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
      </div>
    </div>
    <div class="web-list">
    <h5>移动开发</h5>
      <div class="course">
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
      </div>
    </div><div class="web-list">
    <h5>数据库</h5>
      <div class="course">
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
      </div>
    </div><div class="web-list">
    <h5>云计算</h5>
      <div class="course">
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
      </div>
    </div>
    <div class="web-list">
      <h5>UI设计</h5>
      <div class="course">
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
        <div class="imggg">
          <div class="ices"></div>
          <p>HTML/CSS</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import mHeader from '../../components/header'
  
  export default {
    name: 'broadcast',
    components: {
      mHeader
    }
  }
</script>


<style lang="less">
.appes-list{
  padding-bottom: 21rem;
}
  .web-list{
    h5{
      clear: both;
      color: #AAA;
      padding: .5rem;
      font: .7rem 楷体;
    }
    .course{
      background: #fff;
      padding: .2rem 0 0 .2rem;
      .imggg{
        float: left;
        padding: .5rem 1.43rem;
        .ices{
          height: 2rem;
          width: 2rem;
          background: url("../../assets/images/ic_chat_action_emoji_pressed.png");
          background-repeat: no-repeat;
          background-size: 2rem 2rem;
        }
        p{
          padding-top: .4rem;
          font: .5rem 楷体;
        }
      }
    }
  }
</style>