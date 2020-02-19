<template>
    <section class="share-wrapper">
        <div class="container">
            <div class="row top-center box-wrap">
                <h6>Bagikan jika Anda menyukai halaman ini</h6>
                <div class="share ml-auto">
                    <ul>
                        <li>
                            <span class="icon facebook"><img alt="Vue icon" src="../assets/images/facebook.png"></span>
                            <span class="value">20K</span>
                        </li>
                        <li>
                            <span class="icon twitter"><img alt="Vue icon" src="../assets/images/twitter.png"></span>
                            <span class="value">450</span>
                        </li>
                        <li>
                            <span class="icon gplus"><img alt="Vue icon" src="../assets/images/gplus.png"></span>
                            <span class="value">1900</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'Share'
}
</script>

<style lang="scss">

.share-wrapper {
    background: #F7F7F7;
    padding: 20px 0;
    .top-center {
        align-items: center;
        .share {
            ul {
                display: flex;
                @media(max-width: 480px){
                    justify-content: center;
                }
                li {
                    display: flex;
                    padding-left: 20px;
                    @media(max-width: 480px){
                        padding: 20px 10px 0;
                    }
                    .icon {
                        width: 35px;
                        height: 35px;
                        border-radius: 4px;
                        background: #00AEF1;
                        display: flex;
                        align-items: center;
                        justify-content: center;
                        @media(max-width: 480px){
                            width: 25px;
                            height: 25px;
                            img{
                                width: 15px !important;
                            }
                        }
                        img {
                            width: 20px;
                        }
                    }
                    .facebook {
                        background: #22599b;
                    }
                    .gplus {
                        background: #FC4A34;
                    }
                    .value {
                        border: 1px solid #D7D7D7;
                        border-radius: 4px;
                        width: 60px;
                        display: flex;
                        align-items: center;
                        justify-content: center;
                        position: relative;
                        margin-left: 7px;
                        &:after {
                            content: '';
                            width: 0;
                            height: 0;
                            border-top: 4px solid transparent;
                            border-bottom: 4px solid transparent;
                            border-right: 5px solid #e4e3e3;
                            position: absolute;
                            right: 100%;
                            margin: 0 auto;
                            top: 39%;
                        }
                    }
                }
            }
        }
    }
}

</style>