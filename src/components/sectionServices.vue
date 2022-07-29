<template>

    <div class="sectionServices">
        <div class="container">
            <div class="row justify-content-between">

                <div class="servicesText d-flex flex-column justify-content-center w-25">
                    <span class="txtGreen">OUR BUSINESS AREAS</span>
                    <h1 class="titleNex">Logistics Services</h1>
                    <span class="txtSub">
                        We are leaders in providing logistics services with a set of cutting edge technologies
                        and a team of experienced and renowned professionals.
                    </span>
                    <div class="badges my-3 ">
                        <a href="#" class="mx-1 badge txtBgGreen">Tradition</a>
                        <a href="#" class="mx-1 badge txtBgGreen">Quality</a>
                        <a href="#" class="mx-1 badge txtBgGreen">Security</a>
                    </div>

                    <button id="btnGreen" type="button" class="btn ">READ MORE</button>
                </div>

                <div v-for="(card, index) in servicesCards" :key="index" class="servicesCard mx-3">
                    <img class="img-fluid" src="../assets/img/gallery-3.jpg" alt="card img">
                    <h2> {{ card.title }} </h2>
                    <span> {{ card.desc }} </span>
                </div>

            </div>
        </div>
    </div>

</template>

<script>
export default {
    data: function () {
        return {
            servicesCards: [
                {
                    imgUrl: "gallery-3.jpg",
                    title: "Technology",
                    desc: "Focused on developing technology solutions adapted to our client's needs."
                },
                {
                    imgUrl: "gallery-4.jpg",
                    title: "Transport",
                    desc: "We develop operational strategies to improve logistical efficiency."
                },
            ],
        }
    },
}
</script>


<style scoped lang="scss">
.sectionServices {
    color: black;
    background-color: beige;

    .row {
        padding: 150px 0;

        .servicesText {
            .servicesTitleSmall {
                color: #058182;
                font-weight: bold;
                font-size: .8rem;
            }

            h1 {
                font-weight: bold;
            }

            span {
                color: gray;
                font-size: .8rem;
            }

            div.badges {
                a.badge {
                    color: #058182;
                    text-decoration: none;
                    padding: .6rem .8rem;
                    border-radius: 0;
                }
            }

            button {
                margin: .8rem 0;
                padding: .5rem 0;
                width: 40%;
                font-size: .8rem;
                border-radius: 0;
                background-color: #058182;
                color: white;
            }
        }

        .servicesCard {
            width: 350px;
            background-color: white;
            padding: 3rem;

            img {}

            h2 {
                padding: 1rem 0;
            }

            span {}
        }
    }
}
</style>
