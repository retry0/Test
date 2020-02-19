<template>
    <div class="header-wrapper">
        <div class="top-header">
            <div class="container">
                <div class="row box-wrap">
                    <div class="left">
                        <span class="icon"><img alt="Vue icon" src="../assets/images/price.png"></span>
                        <p>gratis ebook 9 cara cerdas menggunakan domain [ x ]</p>
                    </div>
                    <div class="right ml-auto">
                        <ul>
                            <li>
                                <a href="#">
                                    <span class="icon"><img alt="Vue icon" src="../assets/images/phone.png"></span>
                                    <p>0274-5305505</p>
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    <span class="icon"><img alt="Vue icon" src="../assets/images/chat.png"></span>
                                    <p>live chat</p>
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                <span class="icon"><img alt="Vue icon" src="../assets/images/user.svg"></span>
                                <p>member area</p>
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="navbar-menu">
            <div class="container">
                <div class="row box-wrap">
                    <nav class="navbar navbar-expand-lg ">
                        <a class="navbar-brand" href="#"> <img alt="Vue logo" src="../assets/images/niagahoster-logo.png"></a>
                        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                            <span class="navbar-toggler-icon"><img alt="Vue logo" src="../assets/images/bars.png"></span>
                        </button>

                        <div class="collapse navbar-collapse" id="navbarSupportedContent">
                            <ul class="navbar-nav ml-auto">
                                <li class="nav-item active">
                                    <a class="nav-link" href="#">Hosting <span class="sr-only">(current)</span></a>
                                </li>
                                <li class="nav-item">
                                    <a class="nav-link" href="#">Domain <span class="sr-only">(current)</span></a>
                                </li>
                                <li class="nav-item">
                                    <a class="nav-link" href="#">Server <span class="sr-only">(current)</span></a>
                                </li>
                                <li class="nav-item">
                                    <a class="nav-link" href="#">Website <span class="sr-only">(current)</span></a>
                                </li>
                                <li class="nav-item">
                                    <a class="nav-link" href="#">Afiliasi <span class="sr-only">(current)</span></a>
                                </li>
                                <li class="nav-item">
                                    <a class="nav-link" href="#">Promo <span class="sr-only">(current)</span></a>
                                </li>
                                <li class="nav-item">
                                    <a class="nav-link" href="#">Pembayaran <span class="sr-only">(current)</span></a>
                                </li>
                                <li class="nav-item">
                                    <a class="nav-link" href="#">Review <span class="sr-only">(current)</span></a>
                                </li>
                                <li class="nav-item">
                                    <a class="nav-link" href="#">Kontak <span class="sr-only">(current)</span></a>
                                </li>
                                <li class="nav-item">
                                    <a class="nav-link" href="#">Blog <span class="sr-only">(current)</span></a>
                                </li>
                            </ul>
                        </div>
                    </nav>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Header'
}
</script>

<style lang="scss">
    .top-header{
        border-bottom: 1px solid #F4F4F4;
        padding-bottom: 15px;
        .right {
            ul {
                display: flex;
                position: relative;
                top: 15px;
                li {
                    a{
                        display: flex;
                        padding-left: 20px;
                        align-items: center;
                        .icon {
                            padding-right: 10px;
                            img {
                                width: 20px;
                            }
                        }
                        p{
                            margin-bottom: 0;
                            text-transform: capitalize;
                            font-size: 14px;
                        }

                    }
                }
            }
        }
        .left{
            display: flex;
            align-items: center;
            .icon {
                background: #0090EF;
                text-align: center;
                margin-right: 15px;
                position: relative;
                width: 30px;
                height: 40px;
                padding: 2px 0 0;
                img {
                    width: 18px;
                }
                &:after {
                    content: '';
                    width: 0;
                    height: 0;
                    border-left: 14px solid transparent;
                    border-right: 14px solid transparent;
                    border-bottom: 10px solid #fff;
                    position: absolute;
                    left: 0;
                    right: 0;
                    margin: 0 auto;
                    bottom: 0;
                    @media(max-width: 480px){
                        border-left: 12px solid transparent;
                        border-right: 12px solid transparent;

                    }
                }
            }
            p {
                margin: 0;
                text-transform: capitalize;
                font-size: 14px;
            }
        }

        @media(max-width: 768px){
            .box-wrap {
                display: block;
                @media(max-width: 480px){
                    margin: 0;
                        .right {
                            border-top: 1px solid #eaeaea;
                            margin-top: 10px;
                            ul {
                                display: inline-block;
                                li {
                                    display: inline-block;
                                    padding: 0 10px;
                                }
                            }
                        }
                }
                    .left {
                    justify-content: center;
                }
                .right {
                    ul {
                        justify-content: center;
                        top: 0 !important;
                        padding-top: 10px;
                    }
                }
            }
        }
    }
    .navbar-menu {
        padding: 10px 0;
        border-bottom: 1px solid #f4f4f4;
        @media(max-width: 480px){
            .box-wrap {
                display: block;
                margin: 0;
            }
        }
        .navbar{
            width: 100%;
            padding: 0;
            @media(max-width:1024px){
                display: block ;
            }
            @media(max-width:768px){
                display: flex ;
            }
            .navbar-brand{
                img{
                    width: 300px;
                    @media(max-width: 480px){
                        width: 200px;
                    }
                }
            }
            .navbar-nav {
                @media(max-width: 1024px){
                    margin: 0 auto !important;
                }
            }
            .navbar-toggler {
                background: #27aae1;
                padding: 0px;
                .navbar-toggler-icon {
                    display: flex;
                    align-items: center;
                    justify-content: center;
                }
                img{
                    width: 20px;
                }
            }
            .navbar-collapse{
                ul{
                    padding-top: 20px;
                }
            }
        }
    }

</style>