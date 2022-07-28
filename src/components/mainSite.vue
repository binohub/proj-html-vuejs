<template>
  <div id="mainSite">
    <sectionServices />
    <sectionCompany />
    <sectionLogos />
    <sectionNews />
    <sectionKnow />
  </div>
</template>

<script>
import sectionServices from "../components/sectionServices.vue"
import sectionCompany from "../components/sectionCompany.vue"
import sectionLogos from "../components/sectionLogos.vue"
import sectionNews from "../components/sectionNews.vue"
import sectionKnow from "../components/sectionKnow.vue"
export default {
  components:{
    sectionServices,
    sectionCompany,
    sectionLogos,
    sectionNews,
    sectionKnow,
  }
}
</script>


<style lang="scss">
</style>
