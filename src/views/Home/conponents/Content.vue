<template>
  <div class="content">
    <div class="inner">
      <div class="content-inner">
        <div class="content-header">永不言弃，追求极致。</div>
        <div class="content-body">欢迎小罗伯特·唐尼，<br/> 加入 OnePlus 大家庭。</div>
        <div class="content-button">前往了解 &gt;</div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import '../../../assets/style/scss/custom.scss';

.content{
  background: url('../../../assets/images/content.jpg') center center no-repeat;
  width: 100%;
  height: 300px;
  position: relative;
  overflow: hidden;
  @media screen and (max-width: 700px){
    height: 350px;
    background: url('../../../assets/images/minicontent.jpg') center center no-repeat;
    background-size: cover;
  }
  .inner{
    position: absolute;
    left: 50%;
    width: 100%;
    max-width: 1000px;
    height: 100%;
    transform: translateX(-50%);
    .content-inner{
      position: absolute;
      top: 50%;
      width: 100%;
      max-width: 500px;
      transform: translateY(-50%);
      color: #fff;
      @media screen and (max-width: 700px){
        top: 20%;
        text-align: center;
      }
      .content-header{
        font-size: 30px;
        @media screen and (max-width: 700px){
          font-size: 20px;
        }
      }
      .content-body{
        font-size: $contentSize;
        margin-top: 20px;
        @media screen and (max-width: 700px){
          margin-top: 10px;
          font-size: 16px;
        }
      }
      .content-button{
        font-size: $contentSize;
        margin-top: 40px;
        @media screen and (max-width: 700px){
          margin-top: 10px;
          font-size: 16px;
        }
      }
    }
  }
}
</style>

<script>
export default {
  name: 'HomeContent'
}
</script>
