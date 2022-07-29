<template>

    <div id="sectionKnow">
        <div class="container">
            <div class="row justify-content-between py-5">

                <div class="w-50">
                    <span class="txtGreen">NEWSLETTER</span>
                    <h2 class="txtBgGreen fw-bold text-white">Know First</h2>
                    <span class="txtSub fw-bold">Follow closely and receive content about our company and the news of the current
                        market.</span>
                </div>
                <div class="input&btn w-50">
                    <div class="form-outline my-3">
                        <input type="text" id="form1" class="form-control" placeholder="Name" aria-label="Search" />
                    </div>
                    <div class="form-outline my-3">
                        <input type="mail" id="form1" class="form-control" placeholder="Email" aria-label="Search" />
                    </div>
                    <button id="btnGreen" type="button" class="btn">SUBSCRIBE</button>
                </div>

            </div>
        </div>
    </div>

</template>

<script>
</script>


<style scoped lang="scss">
#sectionKnow{
    background-image: url("../assets/img/bg-1.jpg");
    padding: 8rem 0;
        input{
            border-radius: 0;
            border: 0px;
            width: 60%;
            background: rgb(255, 255, 255, .5)
        }
        button{
            border-radius: 0;
            background-color: green;
            color: white;
        }
}
</style>
