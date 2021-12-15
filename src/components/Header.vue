<template>
  <header>
    <div class="container-1000 header-content">
      <img src="../assets/img/logo-2.png" alt="">
      <div class="nav-bar">
        <ul>
          <!-- dopo aver ciclato gli oggetti, se index è uguale a counter aggiungo la classe active -->
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
          <div class="number-shop">
              0
            </div>
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
  height: 60px;
  background-color: white;
  .header-content{
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    img{
      height: 50px;
    }
    .nav-bar{
      display: flex;
      align-items: center;
      ul{
        list-style: none;
        display: flex;
        align-items: center;
        margin-right: 15px;
        li{
          cursor: pointer;
          line-height: 60px;
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
            font-weight: 600;
          }
        }
      }
      .icon{
        display: flex;
        align-items: center;
        font-size: 15px;
        margin-right: 15px;
        position: relative;
        i{
          padding: 0 8px;
          cursor: pointer;
          transition: all 0.5;
          &:hover{
            transform: scale(1.2);
          }
        }
        .fa-shopping-cart{
          z-index: 99;
        }
        .number-shop{
          position: absolute;
          color: white;
          top: -9px;
          right: -5px;
          padding: 0.5px 5px;
          border-radius: 50%;
          background-color: $primary-color;
          z-index: 1;
        }
      }
      button{
        margin-left: 15px;
      }
    }  
  } 
}
</style>