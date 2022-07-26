<template>

    <div id="headerSite">


        <div id="topHeader">
            <div class="container">
                <div class="row">

                    <div id="topHeaderL">
                    </div>

                    <div id="topHeaderR">
                        <div class="topHeaderNumber"></div>
                        <div class="topHeaderMail"></div>
                        <div class="topHeaderSocial"></div>
                    </div>

                </div>
            </div>
        </div>

        <div id="bottomHeader"></div>


    </div>


</template>

<script>
export default {
    name: 'headerSite',
    props: {
    }
}
</script>


<style scoped lang="scss">
#topHeader {
    height: 5vh;
    background-color: rebeccapurple;
}
</style>
