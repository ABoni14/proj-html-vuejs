<template>
  <section class="container-1000">
    <div class="top">
      <div class="text">
        <h2>Popular features that your business needs</h2>
        <p>Faff about only a quid blower I don't want no agro bleeding chimney <br> pot burke tosser cras nice one boot fanny.!</p>
      </div>
      <button class="button">Explore More Feature</button>
    </div>
    <div class="bottom">
      <div
      v-for="(feature, index) in PopularFeaturesData"
      :key="index"
      class="card">
        <h3>{{feature.text}}</h3>
        <i 
        class="fas" :class="feature.img"></i>
      </div>
    </div>
  </section>
</template>

<script>
import PopularFeaturesData from "../assets/data/PopularFeaturesData"

export default {
  name: "PopularFeatures",

  data(){
    return{
      PopularFeaturesData
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";

section{
    margin-bottom: 60px;
  .top{
    display: flex;
    justify-content: space-between;
    align-items: center;
    .text{
      h2{
        font-size: 30px;
        margin-bottom: 15px;
      }
      p{
        color: $secondary-text-color;
        line-height: 25px;
        margin-bottom: 15px;
      }
    }
  }
  .bottom{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    .card{
      width: calc(100% / 4 - 20px);
      margin: 10px;
      padding: 10px;
      border: 1px solid $border-color;
      box-shadow: 0px 15px 10px $shadow-color;
      h3{
        font-size: 15px;
        font-weight: 500;
        margin-bottom: 20px;
      }
      i{
        font-size: 30px;
        margin-bottom: 20px;
      }
    }
  }
}
</style>