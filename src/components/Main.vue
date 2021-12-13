<template>
  <main>
    <OnlineMarketing />
    <TipsSection />
  </main>
</template>

<script>
import OnlineMarketing from "./OnlineMarketing.vue"
import TipsSection from "./TipsSection.vue"

export default {
  name: "Main",

  components:{
    OnlineMarketing,
    TipsSection
  }
}
</script>

<style lang="scss" scoped>

</style>