<template>

    <div id="sectionLogos" class="d-flex align-items-center">
        <div class="container">
            <div class="row justify-content-between">

                <div class="divLogo" v-for="(item, index) in logoList" :key="index">
                    <img class="img-fluid" src="../assets/img/logo-1.png" alt="logo">
                </div>

            </div>
        </div>
    </div>

</template>

<script>

export default {
    data: function () {
        return {
            logoList: [
                {
                    logoImg: "logo-1.png",
                },
                {
                    logoImg: "logo-2.png",
                },
                {
                    logoImg: "logo-3.png",
                },
                {
                    logoImg: "logo-4.png",
                },
                {
                    logoImg: "logo-5.png",
                },
            ],
        }
    },
}
</script>


<style scoped lang="scss">
#sectionLogos {
    height: 20vh;
    .divLogo{
        width: 200px;
    }
}
</style>
