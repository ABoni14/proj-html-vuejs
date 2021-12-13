<template>
  <main>
    <OnlineMarketing />
    <TipsSection />
    <PopularFeatures />
    <Testimonials />
  </main>
</template>

<script>
import OnlineMarketing from "./OnlineMarketing.vue"
import TipsSection from "./TipsSection.vue"
import PopularFeatures from "./PopularFeatures.vue"
import Testimonials from "./Testimonials.vue"

export default {
  name: "Main",

  components:{
    OnlineMarketing,
    TipsSection,
    PopularFeatures,
    Testimonials
  }
}
</script>

<style lang="scss" scoped>

</style>