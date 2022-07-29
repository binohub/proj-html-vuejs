<template>
    <div id="footerSite">
        <div class="container">
            <div class="row">

                <div id="topFooter">
                    <div id="textFooter">
                        <img class="img-fluid logoNex" src="../assets/img/nexgen-logo-web.png" alt="logo">
                        <span class="txtSub">A Functional HTML Template For Corporate & Business.</span>
                        <div id="number" class="">
                            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                                class="bi bi-telephone-fill" viewBox="0 0 16 16">
                                <path fill-rule="evenodd"
                                    d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.678.678 0 0 0 .178.643l2.457 2.457a.678.678 0 0 0 .644.178l2.189-.547a1.745 1.745 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.634 18.634 0 0 1-7.01-4.42 18.634 18.634 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877L1.885.511z" />
                            </svg>
                            <span class="mx-2">+1 (305) 1234-5678</span>
                        </div>

                        <div id="mail">
                            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                                class="bi bi-envelope-fill" viewBox="0 0 16 16">
                                <path
                                    d="M.05 3.555A2 2 0 0 1 2 2h12a2 2 0 0 1 1.95 1.555L8 8.414.05 3.555ZM0 4.697v7.104l5.803-3.558L0 4.697ZM6.761 8.83l-6.57 4.027A2 2 0 0 0 2 14h12a2 2 0 0 0 1.808-1.144l-6.57-4.027L8 9.586l-1.239-.757Zm3.436-.586L16 11.801V4.697l-5.803 3.546Z" />
                            </svg>
                            <span class="mx-2">hello@example.com</span>
                        </div>
                        <div id="map">
                            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                                class="bi bi-geo-alt-fill" viewBox="0 0 16 16">
                                <path
                                    d="M8 16s6-5.686 6-10A6 6 0 0 0 2 6c0 4.314 6 10 6 10zm0-7a3 3 0 1 1 0-6 3 3 0 0 1 0 6z" />
                            </svg>
                            <span class="mx-2">Main Avenue, 987</span>
                        </div>
                        <button id="btnHide" type="button" class="btn">GET IN TOUCH</button>
                    </div>

                    <div v-for="(item, index) in footerLists" :key="index" class="infoFooter col-2">
                        <h2 class="fw-bold text-white"> {{ item.title }} </h2>
                        <ul class="txtSub">
                            <li>> The Company</li>
                            <li>> Institutional</li>
                            <li>> Social & Events</li>
                            <li>> Innovation</li>
                            <li>> Environment</li>
                            <li>> Technology</li>
                        </ul>
                    </div>
                </div>

                <div id="bottomFooter">
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
@import "../assets/style/var.scss";
@import "../assets/style/general.scss";

#footerSite {
    background-image: url("../assets/img/bg-10.jpg");
    background-position: center;
    background-size: cover;




    #topFooter {
        height: 45vh;
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: space-between;

        #textFooter {
            display: flex;
            flex-direction: column;
            max-width: 300px;
            .txtSub{
                margin-top: 3rem;
            }
            button{
                margin: 1rem 0;

            }
        }

        .infoFooter {
            text-align: left;
            h2{
                font-size: 2rem;
                margin: 2.8rem 0;
                cursor: pointer;
            }
            ul {
                list-style-type: none;
                padding: 0;
                li{
                    margin-top: 1rem;
                    font-size: 1rem;
                    cursor: pointer;
                }
            }
        }
    }

    #bottomFooter {
        display: flex;
        justify-content: space-between;
        align-items: center;


        height: 5vh;
        width: 100%;
        font-size: .8rem;
    }
}
</style>
