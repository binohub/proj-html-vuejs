<template>

    <div id="sectionCompany" class="bg-dark">
        <div class="container">
            <div class="row">

                <div class="w-50 d-flex flex-column justify-content-center">
                    <span class="companyTitle">ABOUT THE NETWORK</span>
                    <h1>The Company</h1>
                    <span>With all of this expertise and capability comes an unrivalled commitment to customer
                        service.</span>

                    <div v-for="(item, index) in companyList" :key="index">
                        <h4>{{ item.title }}</h4>
                        <span>{{ item.desc }}</span>
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

}
</style>
