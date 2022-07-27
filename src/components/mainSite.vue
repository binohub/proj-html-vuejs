<template>
  <div id="mainSite">
    <sectionServices />
    <sectionCompany />
    <sectionLogos />
    <sectionNews />
  </div>
</template>

<script>
import sectionServices from "../components/sectionServices.vue"
import sectionCompany from "../components/sectionCompany.vue"
import sectionLogos from "../components/sectionLogos.vue"
import sectionNews from "../components/sectionNews.vue"
export default {
  components:{
    sectionServices,
    sectionCompany,
    sectionLogos,
    sectionNews,
  }
}
</script>


<style lang="scss">
</style>
