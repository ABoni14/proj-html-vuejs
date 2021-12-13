<template>
  <section class="container-1000">
    <div class="left-content">
      <h2>Get tips tricks on how to skyrocket your sales.</h2>
      <p>Faff about only a quid blower I don't want no agro bleeding chimney pot burke tosser cras nice one boot fanny.!</p>
      <div class="box box-active">
        <img src="../assets/img/510.png" alt="">
        <div class="text-contain">
          <h3>Reporting Analysis</h3>
          <p>It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout.</p>
        </div>
      </div>
      <div class="box">
        <img src="../assets/img/511.png" alt="">
        <div class="text-contain">
          <h3>Reporting Analysis</h3>
          <p>It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout.</p>
        </div>
      </div>
    </div>
    <div class="right-content">
      <img src="../assets/img/509.jpeg" alt="">
    </div>
  </section>
</template>

<script>
export default {
  name: "TipsSection"
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";

section{
  .left-content,
  .right-content{
    float: left;
    width: 50%;
  }
  .left-content{
    padding-right: 20px;
    h2{
      font-size: 35px;
      font-weight: 600;
      margin-bottom: 15px;
    }
    p{
      color: $secondary-text-color;
      font-size: 15px;
      line-height: 25px;
      margin-bottom: 20px;
    }
    .box{
      display: flex;
      align-items: center;
      padding: 10px;
      &.box-active{
        border: 1px solid $border-color;
        box-shadow: 5px 15px 20px $shadow-color;
        margin-bottom: 15px;
      }
      img{
        width: 50px;
        height: 50px;
        margin-right: 10px;
      }
    }
  }
  .right-content{
    img{
      margin-top: 60px;
      width: 100%;
    }
  }
}
</style>