<template>
  <div id="mainSite">
    <div class="sectionServices">
      <div class="container">
        <div class="row">

          <div class="servicesText d-flex flex-column w-25">
            <span class="servicesTitleSmall">OUR BUSINESS AREAS</span>
            <h1>Logistics Services</h1>
            <span>
              We are leaders in providing logistics services with a set of cutting edge technologies
              and a team of experienced and renowned professionals.
            </span>
            <button id="btnGreen" type="button" class="btn">READ MORE</button>
          </div>
          <div class="servicesCard"></div>
          <div class="servicesCard"></div>



        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'mainSite',
  props: {
  }
}
</script>


<style scoped lang="scss">
#mainSite{
  color: black;
  .row{
    margin: 200px 0;
    .servicesText{
      .servicesTitleSmall{
        color: #058182;
        font-weight: bold;
        font-size: .8rem;
      }
      h1{
        font-weight: bold;
      }
      span{
        color: gray;
        font-size: .8rem;
      }
      button{
        margin: .8rem 0;
        padding: .5rem 0;
        width: 40%;
        font-size: .8rem;
        border-radius: 0;
        background-color: #058182;
        color: white;
      }
    }
  }
}
</style>
