<template>
  <div class="xiazai">
    <header>
      <p class="p2">下载</p>
      <div class="titlee">
      <img src="../../assets/images/drawable-xxhdpi-v4/sa.png" style="width: 2.7rem;">
      <img src="../../assets/images/drawable-xxhdpi-v4/ccc.png" style="width: 2.7rem;">
      <img src="../../assets/images/drawable-xxhdpi-v4/zzz.png" style="width: 2.7rem;">
      </div>
    </header>
    <div class="contents-list">
     
        <p class="memory">
          <span>剩余 218.4MB</span> 
          <img class="imgs" src="../../assets/images/ic_rec_group_banner_4.png" > 
          <img class="imges" src="../../assets/images/drawable-xxhdpi-v4/menu_more_icon.png" >
        </p>
       <div class="download">
         <img src="../../assets/images/drawable-xxhdpi-v4/no_downloaded.png" >
         <p>暂无下载内容</p>
       </div>
       <div class="tuijian">
        
       </div>
    <div>
        
      </div>
    </div>
  </div>
</template>

<script>
  import mHeader from '../../components/header'
  
  export default {
    name: 'index',
    components: {
      mHeader
    }
  }
</script>


<style lang="less">
  .xiazai{
    background:#DDD;
    height: 1000rem;
  }
  .contents-list{
    .memory{
      margin-top: .5rem;
      background: #fff;
      padding: .5rem .5rem;
      .imgs{
        padding-right: .1rem;
        width:9rem;
        height:1rem;
      }
      .imges{
        width: 1.5rem;
      }
      span{
        padding-right: .6rem;
      }
    }
    .download{
      text-align: center;
      img{
        margin-top: 2rem;
        width: 6.5rem;
        height: 6.5rem;
      }
    }
  }
</style>