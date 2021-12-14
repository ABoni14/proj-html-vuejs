<template>
  <section class="container-1000">
    <div 
    v-for="(data, index) in OnlineMarketing"
    :key="`top-card${index}`"
    class="card">
      <div class="left-card">
        <img src="../assets/img/24.png" alt="">
      </div>
      <div class="right-card">
        <h3>{{data.title}}</h3>
        <p>{{data.description}}</p>
        <ul>
          <li
          v-for="(role, index) in data.role"
          :key="index"
          >
            <i class="fas fa-check"></i>{{role}}
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script>
import OnlineMarketing from "../assets/data/OnlineMarketingData";

export default {
  name: "OnlineMarketing",

  data(){
    return{
      OnlineMarketing
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";

section{
  display: flex;
  flex-wrap: wrap;
  margin-top: 100px;
  margin-bottom: 100px;
  .card{
    width: calc(100% / 3 - 10px);
    margin: 0 5px;
    height: 100%;
    .left-card{
      float: left;
      width: 20%;
      img{
        width: 100%;
      }
    }
    .right-card{
      padding-left: 8px;
      float: left;
      width: 80%;
      h3{
        font-size: 20px;
        margin-bottom: 10px;
      }
      p{
        color: $secondary-text-color;
        margin-bottom: 10px;
        line-height: 25px;
        font-size: 14px;
        font-weight: 500;
      }
      ul{
        list-style: none;
        li{
          font-weight: 700;
          i{
            color: $primary-color;
            padding: 10px 10px 10px 0;
          }
        }
      }
    }
  }
}
</style>