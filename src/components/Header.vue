<template>
  <header>
    <div class="container-1000 header-content">
      <img src="../assets/img/logo-2.png" alt="">
      <div class="nav-bar">
        <ul>
          <li
          v-for="(listNav, index) in Nav"
          :key="index"
          :class="{active : (index === counter)}"
          @click="counter = index">
            <a href="">{{listNav.text}}</a>
          </li>
        </ul>
        <div class="icon">
          <i class="fas fa-search"></i>
          <i class="fas fa-shopping-cart"></i>
        </div>
        <button class="button">
          Get Started
        </button>
      </div>
    </div>
  </header>
</template>

<script>
import Nav from "../assets/data/ListNavData";

export default {
  name: "Header",

  data(){
    return{
      Nav,
      counter: 0,
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";

header{
  height: 100px;
  background-color: white;
  .header-content{
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    img{
      width: 60px;
    }
    .nav-bar{
      display: flex;
      ul{
        list-style: none;
        display: flex;
        align-items: center;
        margin-right: 15px;
        li{
          cursor: pointer;
          &:hover,
          &.active{
            border-bottom: 2px solid $primary-color;
            margin-bottom: -2px;
          }
          &.active a{
            color: $primary-color;
          }
          a{
            text-decoration: none;
            color: black;
            padding: 0 10px;
            font-size: 15px;
            font-weight: 700;
            height: 100px;
          }
        }
      }
      .icon{
        display: flex;
        align-items: center;
        font-size: 15px;
        margin-right: 15px;
      }
      // .button{
      //   padding: 10px;
      //   background-color: $primary-color;
      // }
    }  
  } 
}
</style>