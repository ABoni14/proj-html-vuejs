<template>
  <section>
    <div class="top">
      <h2>Contact with our team</h2>
      <p>If you are planning on developing a product landing</p>
    </div>
    <div class="bottom container-1000">
      <div class="left">
        <img src="../assets/img/StaticMapService.GetMapIma.png" alt="">
      </div>
      <div class="right">
        <img src="../assets/img/35.png" alt="">
        <h3>9840 Shore St. Fond Du Lac, WI 54935</h3>
        <p>0 1223 456 789<br>mail@sofbox.com</p>
        <div class="icon">
          <i class="fab fa-facebook-f"></i>
          <i class="fab fa-twitter"></i>
          <i class="fab fa-github"></i>
          <i class="fab fa-instagram"></i>
        </div>
        <h2>Get in Touch</h2>
        <form action="">
          <div class="input">
            <input type="text" placeholder="Your Name">
            <input type="text" placeholder="Your Email">
          </div>
          <input type="text" class="subject" placeholder="Your Subject">
          <textarea name="" id="" cols="30" rows="10" placeholder="Your Message"></textarea>
          <input type="submit" value="Send Message" class="button">
        </form>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ContactTeam"
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";

section{
  padding-bottom: 100px;
  border-bottom: 1px solid $border-color;
  .top{
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 25px;
    h2, p{
      margin-bottom: 25px;
    }
    p{
      color: $secondary-text-color;
    }
  }
  .bottom{
    display: flex;
    justify-content: space-between;
    .left{
      width: 50%;
      img{
        width: 100%;
      }
    }
    .right{
      width: 50%;
      padding-left: 25px;
      img, p, .icon{
        margin-bottom: 40px;
      }
      h3, h2{
        margin-bottom: 20px;
      }
      p{
        color: $secondary-text-color;
      }
      .icon i{
        color: $primary-color;
        font-size: 20px;
        padding: 20px;
        border: 1px solid $border-color;
        margin-right: 10px;
        border-radius: 5px;
        cursor: pointer;
      }
      input, textarea{
        padding: 10px;
        border-radius: 5px;
        border: 1px solid $border-color;
      }
      .input{
        display: flex;
        justify-content: space-between;
        input{
          width: 48%;
        }
      }
      .subject, textarea{
        display: block;
        margin: 20px 0;
        width: 100%;
      }

    }
  }
}

</style>