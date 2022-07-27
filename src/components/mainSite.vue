<template>
  <div id="mainSite">
    <sectionServices />
    <sectionCompany />
    <sectionLogos />
  </div>
</template>

<script>
import sectionServices from "../components/sectionServices.vue"
import sectionCompany from "../components/sectionCompany.vue"
import sectionLogos from "../components/sectionLogos.vue"
export default {
  components:{
    sectionServices,
    sectionCompany,
    sectionLogos,
  }
}
</script>


<style lang="scss">
</style>
