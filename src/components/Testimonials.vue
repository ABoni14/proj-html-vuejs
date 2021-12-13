<template>
  <section>
    <div class="contain-text">
      <h2>Our Testimonials</h2>
      <p>If you are planning on developing a product landing app or website, <br>take a look at this beatiful-crafted</p>
    </div>
    <div class="contain-card container-1000">
      <div class="card"></div>
      <div class="card"></div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Testimonials"
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";

section{
  
  .contain-text{
    background-image: url("../assets/img/15.png");
    background-color: $secondary-bg;
    background-size: cover;
    background-position:center;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    text-align: center;
    padding-bottom: 50px;
    h2{
      font-size: 30px;
      margin-bottom: 20px;
    }
    p{
      color: $secondary-text-color;
      line-height: 25px;
    }
  }
  .contain-card{
    display: flex;
    justify-content: space-between;
    background-color: blue;
    .card{
      width: 399px;
      height: 500px;
      background-color: red;
    }
  }
}
</style>