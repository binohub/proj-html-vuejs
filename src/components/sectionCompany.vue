<template>

    <div id="sectionCompany" class="bg-dark">
        <div class="container">
            <div class="row">

                <div class="w-50 d-flex flex-column justify-content-center">
                    <span class="txtGreen">ABOUT THE NETWORK</span>
                    <div class="d-flex align-items-center">
                        <h1 class="txtBgGreen fw-bold">The </h1>
                        <h1 class="fw-bold">Company</h1>
                    </div>

                    <span class="txtSub">With all of this expertise and capability comes an unrivalled commitment to customer
                        service.</span>

                    <div class="liCompany" v-for="(item, index) in companyList" :key="index">
                        <h4 class="fw-bold">{{ item.title }}</h4>
                        <span class="txtSub">{{ item.desc }}</span>
                    </div>

                </div>
                <div class="w-50">
                    <img class="img-fluid" src="../assets/img/about-5.jpg" alt="company img">
                </div>

            </div>
        </div>
    </div>

</template>

<script>

export default {
    data: function () {
        return {
            companyList: [
                {
                    title: "Leadership",
                    desc: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Obcaecati facere at saepe voluptatem dolorum dolores necessitatibus delectus et porro veritatis culpa quidem quae sed, blanditiis ab nihil fugiat. Dolores, magni."
                },
                {
                    title: "Psychology",
                    desc: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Obcaecati facere at saepe voluptatem dolorum dolores necessitatibus delectus et porro veritatis culpa quidem quae sed, blanditiis ab nihil fugiat. Dolores, magni."
                },
                {
                    title: "Flexibility",
                    desc: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Obcaecati facere at saepe voluptatem dolorum dolores necessitatibus delectus et porro veritatis culpa quidem quae sed, blanditiis ab nihil fugiat. Dolores, magni."
                },
            ],
        }
    },
}
</script>


<style scoped lang="scss">
#sectionCompany {

    span {
        font-size: .6rem;
    }
    .liCompany{
        padding-left: 5rem;
        padding-top: 2rem;
        padding-right: 10rem;
    }

}
</style>
