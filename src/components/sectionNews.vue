<template>

    <div id="sectionNews">
        <div class="container">
            <div class="row justify-content-between py-5">

                <span class="txtGreen">OUR EDITORIAL CONTENT</span>
                <div class="d-flex align-items-center">
                    <h2 class="titleNex">Latest </h2>
                    <h2 class="titleNex txtBgGreen">News</h2>
                </div>

                <div class="col-12 d-flex justify-content-between">
                    <span class="txtSub">Every week we publish content about what is best in the business world.</span>
                    <button id="btnGreen" type="button" class="btn">SEE ALL</button>
                </div>
                <div v-for="(card, index) in newsCards" :key="index" class="square position-relative">
                    <h4 class="position-absolute">{{ card.title }}</h4>
                    <img class="img-fluid" src="../assets/img/news-1.jpg" alt="news img">
                </div>


            </div>
        </div>
    </div>

</template>

<script>
export default {
    data: function () {
        return {
            newsCards: [
                {
                    title: "Increasing creativity is possible for everyone",
                    backCard: "../assets/img/news-1.jpg",
                },
                {
                    title: "Because market research is part of the business plan",
                    backCard: "../assets/img/news-2.jpg",
                },
                {
                    title: "Working from home is now a trend",
                    backCard: "../assets/img/news-3.jpg",
                },
            ],
        }
    },
}
</script>


<style scoped lang="scss">
#sectionNews {
    color: black;


    div {
        button {
            background-color: #058182;
            color: white;
            border-radius: 0;
            font-size: .8rem;
            padding: .5rem 1rem;
        }
    }

    div.square {
        height: 300px;
        width: 350px;
        margin: 2rem 0;

        h4 {
            color: white;
            font-weight: bold;
            bottom: 0px;
            padding: 0 2rem;
            font-size: 1.2rem;
            z-index: 2;
            text-align: center;
        }

        img {
            filter: brightness(.5);
            border-radius: 20px;
        }
    }
}
</style>
