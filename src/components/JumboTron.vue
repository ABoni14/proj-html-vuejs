<template>
  <section class="container-1100">
    <div class="left-section">
      <h2>The biggest platform for your growth.</h2>
      <p>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form</p>
      <button class="button">Read More</button>
    </div>
    <div class="right-section">
      <img src="../assets/img/27-1.png" alt="">
    </div>
  </section>
</template>

<script>
export default {
  name: "JumboTron"
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";

section{
  height: 380px;
  margin-top: 20px;
  background-color: $secondary-bg;
  .left-section,
  .right-section{
    float: left;
    width: 50%;
  }
  .left-section{
    padding: 45px;
    h2{
      font-size: 50px;
      font-weight: 400;
      line-height: 70px;
      padding-bottom: 20px;
    }
    p{
      color: $secondary-text-color;
      line-height: 25px;
      padding-bottom: 20px;
    }
  }
  .right-section{
    padding: 20px;
    img{
      width: 100%;
    }
  }
  
}
</style>