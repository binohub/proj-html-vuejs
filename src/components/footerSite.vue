<template>
    <div id="footerSite">
        <div class="container">
            <div class="row">

                <div id="topFooter" class="d-flex justify-content-between">
                    <div id="textFooter" class="col-2">
                        <img class="img-fluid" src="../assets/img/nexgen-logo-web.png" alt="logo">
                        <span>A Functional HTML Template For Corporate & Business.</span>
                        <div id="topHeaderNumber" class="my-2">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="currentColor"
                                class="bi bi-telephone-fill" viewBox="0 0 16 16">
                                <path fill-rule="evenodd"
                                    d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.678.678 0 0 0 .178.643l2.457 2.457a.678.678 0 0 0 .644.178l2.189-.547a1.745 1.745 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.634 18.634 0 0 1-7.01-4.42 18.634 18.634 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877L1.885.511z" />
                            </svg>
                            <span class="mx-2">+1 (305) 1234-5678</span>
                        </div>
                        <div id="topHeaderMail" class="">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="currentColor"
                                class="bi bi-envelope-fill" viewBox="0 0 16 16">
                                <path
                                    d="M.05 3.555A2 2 0 0 1 2 2h12a2 2 0 0 1 1.95 1.555L8 8.414.05 3.555ZM0 4.697v7.104l5.803-3.558L0 4.697ZM6.761 8.83l-6.57 4.027A2 2 0 0 0 2 14h12a2 2 0 0 0 1.808-1.144l-6.57-4.027L8 9.586l-1.239-.757Zm3.436-.586L16 11.801V4.697l-5.803 3.546Z" />
                            </svg>
                            <span class="mx-2">hello@example.com</span>
                        </div>
                        <button type="button" class="btn btn-outline-success text-white my-2">GET IN TOUCH</button>
                    </div>
                    <div v-for="(item, index) in footerLists" :key="index" class="infoFooter col-2">
                        <h2 class="fw-bold text-white"> {{ item.title }} </h2>
                        <ul class="">
                            <li>> The Company</li>
                            <li>> Institutional</li>
                            <li>> Social & Events</li>
                            <li>> Innovation</li>
                            <li>> Environment</li>
                            <li>> Technology</li>
                        </ul>
                    </div>
                </div>

                <div id="bottomFooter" class="d-flex justify-content-between align-items-center">
                    <span class="text-left">Enjoy the low price. We are tracking any intentions of privacy</span>
                    <span class="text-right">© 2020 NEXGEN is Proudly Powered by <a href="#">Codings</a></span>
                </div>

            </div>
        </div>
    </div>
</template>

<script>
export default {
    data: function () {
        return {
            footerLists: [
                {
                    title: "About",
                },
                {
                    title: "Transport",
                },
                {
                    title: "Support",
                },
            ],
        }
    },
}
</script>


<style scoped lang="scss">
#footerSite {
    background-color: black;
    color: white;
    background-image: url("../assets/img/bg-10.jpg");

    #topFooter {
        padding: 100px 0px;
        color: lightgray;

        #textFooter {
            img {
                filter: invert(2);
            }
        }

        .infoFooter {
            text-align: left;

            ul {
                list-style-type: none;
                padding: 0;
            }
        }
    }

    #bottomFooter {
        height: 5vh;
        font-size: .8rem;
    }
}
</style>
