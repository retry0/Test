<template>
    <section class="hosting-wrapper">
        <div class="container">
            <div class="row box-wrap">
                <div class="col-md-6 col-sm-6 col-xs-12 m-fw text">
                    <div class="left-text">
                        <h3 class="title">Linux Hosting yang Stabil dengan teknologi LVE</h3>
                        <p class="sub-title">
                            SuperMicro <strong>Intel Xeon 24-Cores</strong>  server dengan RAM <strong>128GB</strong>
                            dan teknologi <strong>LVE CloudLinux</strong> untuk stabilitas server Anda. Dilengkapi dengan <strong>SSD</strong>
                            untuk kecepatan <strong>MySQL</strong> dan chacing, Apache load balancer berbasis LiteSpeed Technologies,
                            <strong>CageFS</strong> security, <strong>Raid-10</strong> protection dan auto backup untuk keamanan website Anda.
                        </p>
                        <p class="small">Nb. Composer dan SSH hanya tersediapada paket Personal dan Bisnis</p>
                        <button class="btn btn-rounded btn-solid-blue">Pilih Hosting Anda</button>
                    </div>
                </div>
                <div class="col-md-6 col-sm-6 col-xs-12 m-fw images">
                    <div class="right-image">
                        <img alt="Vue logo" src="../assets/images/image-support.png">
                    </div>
                </div>
            </div>
        </div>

    </section>
</template>
<script>
export default {
    name: 'LinuxHosting'
}
</script>

<style lang="scss" scoped>
.hosting-wrapper{
    .right-image{
         img {
            position: relative;
            top: 71px;
            width: 100%;
            @media(max-width:768px){
                top: 0;
            }
        }
    }
}
</style>