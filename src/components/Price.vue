<template>
    <section class="pricing-wrapper">
        <div class="container">
            <div class="row flex-end">
                <h2 class="title"><strong>Paket Hosting Singapura yang Tepat</strong></h2>
                <h4 class="center">Diskon 40% + Domain dan SSL Gratis untuk Anda</h4>
                <div v-for="pricing in pricing" :key="pricing" class="card card-pricing">
                    <div class="package-name border-bottom ">
                        <h3><strong>{{pricing.package}}</strong></h3>
                    </div>
                    <div class="pricing border-bottom">
                        <h6><span class="small">Rp.</span> {{pricing.oldprice}}</h6>
                        <h3><span class="small">Rp.</span> <strong>{{pricing.newprice}}</strong> <span class="small">/bln</span></h3>
                    </div>
                    <div class="user border-bottom">
                        <p><strong>{{pricing.userregistered}}</strong> Pengguna Terdaftar</p>
                    </div>
                    <div class="feature">
                        <p><strong>{{pricing.power}}</strong></p>
                        <p>{{pricing.bandwith}}</p>
                        <p>{{pricing.email}}</p>
                        <p>{{pricing.db}}</p>
                        <p>{{pricing.addon}}</p>
                        <p>{{pricing.backup}}</p>
                        <p>{{pricing.domain}}</p>
                        <p>{{pricing.ssl}}</p>
                        <p>{{pricing.server}}</p>
                        <p>{{pricing.priority}}</p>
                        <p>{{pricing.rate}}</p>
                        <p>{{pricing.protection}}</p>
                    </div>
                    <button class="btn btn-outline-black">{{pricing.button}}</button>
                    <span class="ribbon ribbon-top-left"><p class="content">Best Seller !</p></span>
                </div>
            </div>
        </div>
        
    </section>
</template>
<script>
import axios from 'axios'
export default {
    name: 'Pricing',
    data(){
    return {
      pricing : [],
      feature: []

    }
  },
    mounted() {
      axios.get("http://localhost:3000/pricing")
      .then(response => {this.pricing = response.data})
    }
  }

</script>

<style lang="scss" scoped>
.pricing-wrapper{
    .flex-end{
        align-items: end;
    }
    .title {
        padding-bottom: 10px;
    }
    .center{
        width: 100%;
    }
    .card-pricing {
        width: 25%;
        margin-top: 70px;
        @media(max-width: 768px){
            width: 50%;
        }
        @media(max-width: 480px){
            width: 100%;
        }
        h6 {
            position: relative;
            display: inline-block;
            padding-bottom: 5px;
            &:after {
                content: '';
                position: absolute;
                top: 50%;
                bottom: 0;
                height: 1px;
                width: 100%;
                background: #2d3e50;
                left: 0;
            }
        }
        .border-bottom {
            padding: 10px 0;
        }
        .feature {
            padding-top: 20px;
            p {
                font-size: 14px;
                padding-bottom: 7px;
            }
        }
        .btn {
            width: unset;
            font-size: 14px !important;
            margin: 30px auto;
        }
        &:nth-of-type(3){
            border-color: #008FEE;
            .ribbon{
                visibility: visible;
            }
            .package-name {
                background: #008fee;
                color: #fff;
                border: 0 !important;
            }
            .pricing {
                background: #008fee;
                color: #fff;
                border: 0 !important;
                h6 {
                    &:after {
                        content: '';
                        background: #fff;
                    }
                }
            }
             .user {
                background: #007ede;
                color: #fff;
            }
            .btn {
                background: #007ede;
                border-color: #007ede !important;
                color: #fff;
            }
        }

    }
    .ribbon {
        width: 105px;
        height: 105px;
        overflow: hidden;
        position: absolute;
        top: -10px;
        left: -10px;
        visibility: hidden;
        &:before, &:after{
            position: absolute;
            z-index: 0;
            content: '';
            display: block;
            border: 5px solid #04924a;
            border-top-color: transparent;
            border-left-color: transparent;
        }
        &:before{
            top: 0;
            right: 0;
        }
        &:after{
            bottom: -1px;
            left: -1px;
        }
        .content {
            position: absolute;
            display: block;
            width: 170px;
            padding: 15px 0;
            background-color: #00B359;
            box-shadow: 0 5px 10px rgba(0,0,0,.1);
            color: #fff;
            text-shadow: 0 1px 1px rgba(0,0,0,.2);
            text-transform: uppercase;
            text-align: center;
            right: -18px;
            top: 12px;
            transform: rotate(-45deg);
            font-size: 11px;
            font-weight: 700;
        }
    }
}


</style>