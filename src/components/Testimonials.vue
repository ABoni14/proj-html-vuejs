<template>
  <section>
    <div class="contain-text">
      <h2>Our Testimonials</h2>
      <p>If you are planning on developing a product landing app or website, <br>take a look at this beatiful-crafted</p>
    </div>
    <div class="contain-card container-1000">
      <div class="card">
        <img src="../assets/img/26.jpeg" alt="">
        <h4>Julia Aann <span>- COO Sofbox</span></h4>
        <p>At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.</p>
        <div class="apici">
          <i class="fas fa-quote-left"></i>
        </div>
      </div>
      <div class="card">
        <img src="../assets/img/27.jpeg" alt="">
        <h4>Mac Znder <span>- Manager Sofbox</span></h4>
        <p>At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.</p>
      </div>
    </div>
    <div class="circle-contain container-1000">
      <div class="circle"></div>
      <div class="circle circle-active"></div>
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
  margin-bottom: 30px;
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
    padding-bottom: 130px;
    padding-top: 130px;
    margin-bottom: 30px;
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
    .card{
      width: 450px;
      padding: 30px 15px;
      text-align: center;
      border: 1px solid $border-color;
      box-shadow: 0px 15px 10px $shadow-color;
      position: relative;
      z-index: 1;
      img{
        width: 70px;
        border-radius: 50%;
        margin-bottom: 30px;
      }
      h4{
        margin-bottom: 30px;
        position: relative;
        z-index: 99;
        span{
          color: $secondary-text-color;
          font-weight: 500;
        }
      }
      p{
        color: $secondary-text-color;
        text-align: start;
        line-height: 25px;
        position: relative;
        z-index: 98;
      }
      .apici{
        width: 100%;
        height: 100%;
        position: absolute;
        z-index: 3;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        i{
          font-size: 100px;
          position: absolute;
          color: $border-color;
          z-index: 5;
          transform: rotate(180deg);
        } 
      }
    }
  }
  .circle-contain{
    display: flex;
    justify-content: center;
    margin-top: 25px;
    .circle{
      width: 8px;
      height: 8px;
      border-radius: 50%;
      background-color: $primary-color;
      margin: 3px;
      cursor: pointer;
      &.circle-active{
        background-color: #1e1e1e;
      }
    }
  }
}
</style>