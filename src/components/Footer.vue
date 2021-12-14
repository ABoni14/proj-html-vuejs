<template>
  <footer class="container-1000">
    <div class="left">
      <img src="../assets/img/35.png" alt="">
      <p>It is a long established fact that a reader will be distracyed by the readable content</p>
      <span>Copyright @2018 <a href="#">Sofbox</a></span>
    </div>
    <div class="right">
      <div
      v-for="(menu, index) in FooterListData" 
      :key="`menu${index}`"
      class="list">
        <h4>{{menu.title}}</h4>
        <ul>
          <li 
          v-for="(list, index) in menu.list"
          :key="index">
            <a href="">{{list}}</a>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
import FooterListData from "../assets/data/FooterListData"

export default {
  name: "Footer",

  data(){
    return{
      FooterListData,
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";

footer{
  display: flex;
  padding: 50px 0;
  .left{
    width: 30%;
    margin-right: 100px;
    img{
      width: 130px;
      margin-bottom: 10px;
      cursor: pointer;
    }
    p{
      color: $secondary-text-color;
      margin-bottom: 70px;
    }
    span{
      color: $secondary-text-color;
      a{
        text-decoration: none;
        color: $primary-color;
        font-weight: 600;
        cursor: pointer;
      }
    }
  }
  .right{
    width: 70%;
    display: flex;
    flex-wrap: wrap;
    padding-left: 30px;
    .list{
      width: calc(100% / 3 - 60px);
      margin: 0 30px;
      h4{
        margin-bottom: 20px;
      }
      ul li{
        list-style: none;
        padding: 9px 0;
        a{
          color: $secondary-text-color;
          text-decoration: none;
        }
      }
    }
  }
}
</style>