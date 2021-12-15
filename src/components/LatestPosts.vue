<template>
  <section>
    <div class="container-1000">
      <div class="top">
        <h2>Latest Posts</h2>
        <p>If you are planning on developing a product landing.</p>
      </div>
      <div class="bottom">
        <div 
        v-for="(post, index) in LatestPostsData"
        :key="index"
        class="card">
          <div class="top-card">
            <img :src="post.img" alt="">
            <div class="date">
              {{post.data}}
            </div>
          </div>
          <div class="bottom-card">
            <h3>{{post.title}}</h3>
            <p>{{post.description}}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import LatestPostsData from "../assets/data/LatestPostsData"

export default {
  name: "LatestPosts",

  data(){
    return{
      LatestPostsData
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";

section{
  margin-top: 100px;
  margin-bottom: 100px;
  .top{
    display: flex;
    align-items: center;
    flex-direction: column;
    margin-bottom: 30px;
    p{
      color: $secondary-text-color;
      margin-top: 20px;
      margin-bottom: 30px;
    }
  }
  .bottom{
    display: flex;
    justify-content: space-between;
    .card{
      width: calc(100% / 3 - 20px);
      border: 1px solid $border-color;
      transition: all 0.5s;
      cursor: pointer;
      &:hover{
        transform: scale(1.1);
      }
      .top-card{
        padding: 5px;
        position: relative;
        img{
          width: 100%;
        }
        .date{
          position: absolute;
          top: 10px;
          left: 10px;
          background-color: $border-color;
          color: $secondary-text-color;
          padding: 7px;
          border-radius: 5px;
          font-size: 12px;
        }
      }
      .bottom-card{
        padding: 15px;
        h3{
          margin-bottom: 15px;
        }
        p{
          color: $secondary-text-color
        }
      }
    }
  }
}
</style>