<template>
  <section>
    <div class="top">
      <h2>Contact with our team</h2>
      <p>If you are planning on developing a product landing</p>
    </div>
    <div class="bottom container-1000">
      <div class="left">
        <img src="../assets/img/StaticMapService.GetMapIma.png" alt="">
        <div class="icon-maps">
          <div class="directions">
            <div class="contain">
              <div class="left-box">
                <h4>Storey Ave</h4>
                <p>San Francisco, California 94129</p>
                <a href="">Visualizza mappa più grande</a>
              </div>
              <div class="right-box">
                <img src="../assets/img/road.png" alt="">
                <a href="">Indicazi...</a>
              </div>
            </div> 
          </div>
          <div class="maps-data">
            <span>Dati mappa @2020</span>
            <span>Termini e condizioni d'uso</span>
            <span>Segnala un errore nella mappa</span>
          </div>
          <div class="maps-button">
            <i class="fas fa-plus border"></i>
            <i class="fas fa-minus"></i>
          </div>
          <div class="red-point">
            <img src="../assets/img/red-point.png" alt="">
          </div>
          <div class="miniature">
            <img src="../assets/img/miniatur-maps.jpg" alt="">
          </div>
        </div>
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
      height: 405px;
      position: relative;
      img{
        width: 100%;
      }
      .icon-maps{
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        z-index: 100;
        .directions{
          position: absolute;
          top: 8px;
          left: 8px;
          padding: 12px;
          z-index: 101;
          background-color: white;
          border-radius: 5px;
          border: 1ps solid $border-color;
          .contain{
            display: flex;
            justify-content: space-between;
            font-weight: 600;
            .left-box{
              margin-right: 60px;
              h4{
                margin-bottom: 8px;
              }
              p, a{
                font-size: 12px;
              }
              p{
                color: $secondary-text-color;
                margin-bottom: 15px;
              }
              a{
                color: $primary-color;
                text-decoration: none;
              }
            }
            .right-box{
              display: flex;
              flex-direction: column;
              align-items: center;
              img{
                width: 25px;
              }
              a{
                font-size: 10px;
                display: block;
                color: $primary-color;
                font-weight: 600;
              }
            }
          }
        }
      }
      .maps-data{
        position: absolute;
        bottom: 0;
        right: 0;
        span{
          font-size: 10px;
          padding: 1px;
          background-color: rgba(255, 255, 255, 0.5);
          margin-left: 3px;
          font-weight: 600;
        }
      }
      .maps-button{
        position: absolute;
        right: 8px;
        bottom: 20px;
        border: 1px solid $shadow-color;
        cursor: pointer;
        i{
          display: block;
          padding: 7px;
          background-color: $border-color;
          color: rgb(92, 92, 92);
          font-size: 20px;
          &.border{
            border-bottom: 1px solid lightgrey;
          }
        }
      }
      .red-point{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        img{
          width: 25px;
          background-image: none;
        }
      }
      .miniature{
        position: absolute;
        left: 8px;
        bottom: 20px;
        width: 40px;
        height: 40px;
        border: 2px solid white;
        overflow: hidden;
        cursor: pointer;
        img{
          width: 100%;
          height: 100%;
          object-fit: cover;

        }
      }
    }
    .right{
      width: 50%;
      padding-left: 25px;
      img, p, .icon{
        margin-bottom: 40px;
      }
      img{
        cursor: pointer;
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
        transition: all 0.5s;
        &:hover{
          color: black;
        }
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