<template>
    <section class="package-wrapper small-underline">
        <div class="container">
            <div class="row">
                <h2 class="title">Semua Paket Hosting Sudah Termasuk</h2>
                <div class="col-md-4 col-sm-6 col-xs-12">
                    <div class="card">
                        <span class="icon"><img alt="Vue icon" src="../assets/images/phpversion.svg"></span>
                        <h5><strong>PHP Semua Versi</strong></h5>
                        <p>Pilih semua dari versi PHP 5.3 s/d PHP 7. Ubah sesuka Anda</p>
                    </div>
                </div>
                <div class="col-md-4 col-sm-6 col-xs-12">
                    <div class="card">
                        <span class="icon"><img alt="Vue icon" src="../assets/images/database.svg"></span>
                        <h5><strong>MySQL Versi 5.6</strong></h5>
                        <p>Nikmati MySQL versi terbaru, tercepat dan kaya akan fitur</p>
                    </div>
                </div>
                <div class="col-md-4 col-sm-6 col-xs-12">
                    <div class="card">
                        <span class="icon"><img alt="Vue icon" src="../assets/images/cpanel.svg"></span>
                        <h5><strong>Panel Hosting cPanel</strong></h5>
                        <p>Kelola website dengan panel canggih yang familiar di hati Anda</p>
                    </div>
                </div>
                <div class="col-md-4 col-sm-6 col-xs-12 bottom">
                    <div class="card">
                        <span class="icon"><img alt="Vue icon" src="../assets/images/guarantee.svg"></span>
                        <h5><strong>Garansi Uptime 99,9%</strong></h5>
                        <p>Data center yang mendukung kelangsungan Anda 24/7</p>
                    </div>
                </div>
                <div class="col-md-4 col-sm-6 col-xs-12 bottom">
                    <div class="card">
                        <span class="icon"><img alt="Vue icon" src="../assets/images/innodb.svg"></span>
                        <h5><strong>Database InnoDB Unlimited</strong></h5>
                        <p>Jumlah dan ukuran database yang tumbuh sesuai kebutuhan Anda.</p>
                    </div>
                </div>
                <div class="col-md-4 col-sm-6 col-xs-12 bottom">
                    <div class="card">
                        <span class="icon"><img alt="Vue icon" src="../assets/images/remote.svg"></span>
                        <h5><strong>Wildcard Remote MySQL</strong></h5>
                        <p>Mendukung s/d 25 max_user_connections dan 1-- max_connections.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'Package'
}
</script>
<style lang="scss">
.package-wrapper {
    .card {
        border: 0;
        .icon {
            padding-bottom: 15px;
            img {
                width: 80px;
            }
        }
    }
    .bottom {
    padding-top: 100px;
    @media(max-width: 480px){
        padding: 0;
    }
}
}
</style>