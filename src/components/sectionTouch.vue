<template>

    <div id="sectionTouch">
        <div class="container">
            <div class="row">

                <div class="touchL w-50">
                    <span class="txtGreen">SEND A MESSAGE</span>
                    <div class="bigTitleNex">
                        <span class="titleNex">Get in </span>
                        <span class="titleNex txtBgGreen">Touch</span>
                    </div>
                    <span class="txtSub">We will respond to your message as soon as possible</span>

                    <div class="form-outline">
                        <input type="text" id="inputGray" class="form-control" placeholder="Name" aria-label="Search" />
                        <input type="mail" id="inputGray" class="form-control" placeholder="Email"
                            aria-label="Search" />
                    </div>

                    <div class="form-outline">
                        <input type="text" id="inputGray" class="form-control" placeholder="Phone"
                            aria-label="Search" />
                        <input type="mail" id="inputGray" class="form-control" placeholder="More Info"
                            aria-label="Search" />
                    </div>
                    <div class="form-outline">
                        <textarea class="textArea" placeholder="Message" name="message" id="inputGray" cols="30"
                            rows="10"></textarea>
                    </div>

                    <button id="btnGreen" type="button" class="btn btn-success">SUBSCRIBE</button>
                </div>
                <div class="touchR w-50">
                    <h2 class="fw-bold">Example Inc.</h2>
                    <span class="txtSub">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Dolorum quis magni
                        facere hic! Minus
                        tenetur suscipit aspernatur eveniet!</span>
                    <span class="txtSub">Praesent diam lacus, dapibus sed imperdietdap bus sed imperdiet
                        consececteur.</span>
                    <div id="number" class="">
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                            class="txtGreen bi bi-telephone-fill" viewBox="0 0 16 16">
                            <path fill-rule="evenodd"
                                d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.678.678 0 0 0 .178.643l2.457 2.457a.678.678 0 0 0 .644.178l2.189-.547a1.745 1.745 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.634 18.634 0 0 1-7.01-4.42 18.634 18.634 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877L1.885.511z" />
                        </svg>
                        <span class="txtGreen mx-2">+1 (305) 1234-5678</span>
                    </div>
                    <div id="mail">
                        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="currentColor"
                            class="txtGreen bi bi-envelope-fill" viewBox="0 0 16 16">
                            <path
                                d="M.05 3.555A2 2 0 0 1 2 2h12a2 2 0 0 1 1.95 1.555L8 8.414.05 3.555ZM0 4.697v7.104l5.803-3.558L0 4.697ZM6.761 8.83l-6.57 4.027A2 2 0 0 0 2 14h12a2 2 0 0 0 1.808-1.144l-6.57-4.027L8 9.586l-1.239-.757Zm3.436-.586L16 11.801V4.697l-5.803 3.546Z" />
                        </svg>
                        <span class="txtGreen mx-2">hello@example.com</span>
                    </div>
                    <div id="map">
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                            class="txtGreen bi bi-geo-alt-fill" viewBox="0 0 16 16">
                            <path
                                d="M8 16s6-5.686 6-10A6 6 0 0 0 2 6c0 4.314 6 10 6 10zm0-7a3 3 0 1 1 0-6 3 3 0 0 1 0 6z" />
                        </svg>
                        <span class="txtGreen mx-2">Main Avenue, 987</span>
                    </div>
                    
                    <button id="btnHide" type="button" class="btn btn-success">VIEW MAP</button>
                </div>

            </div>
        </div>
    </div>

</template>

<script>
</script>


<style scoped lang="scss">
@import "../assets/style/var.scss";
@import "../assets/style/general.scss";

#sectionTouch {
    background-color: $Saltpan;
    color: $OuterSpace;

    .row {
        align-items: center;

        .touchL {
            display: flex;
            flex-direction: column;
            margin: 5rem 0;

            .form-outline {
                display: flex;
                justify-content: space-between;

                .textArea {
                    width: 100%;
                }
            }
        }

        .touchR {
            display: flex;
            flex-direction: column;
            padding: 0 5rem;
            button{
                color: $ElfGreen;
            }
        }

    }
}
</style>
