<template>
  <main>
    <OnlineMarketing />
    <TipsSection />
    <PopularFeatures />
    <Testimonials />
    <LatestPosts />
    <ContactTeam />
  </main>
</template>

<script>
import OnlineMarketing from "./OnlineMarketing.vue"
import TipsSection from "./TipsSection.vue"
import PopularFeatures from "./PopularFeatures.vue"
import Testimonials from "./Testimonials.vue"
import LatestPosts from "./LatestPosts.vue"
import ContactTeam from "./ContactTeam.vue"

export default {
  name: "Main",

  components:{
    OnlineMarketing,
    TipsSection,
    PopularFeatures,
    Testimonials,
    LatestPosts,
    ContactTeam
  }
}
</script>

<style lang="scss" scoped>

</style>