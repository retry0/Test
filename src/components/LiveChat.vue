<template>
    <section class="livechat-wrapper">
        <div class="container">
            <div class="row align-center">
                <h2>Perlu <strong>BANTUAN?</strong>  Hubungi kami : <strong>0274-5305505</strong></h2>
                <button class="btn btn-outline-white ml-auto"> <img alt="Vue logo" src="../assets/images/chat-white.png">Live Chat</button>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'LiveChat'
}
</script>
<style lang="scss">
.livechat-wrapper {
    background: #2b8cea;
    color: #fff;
    .btn {
        margin-top: 0;
        color: #fff;
        img {
            width: 30px;
            margin-right: 10px;
        }
    }
    .align-center {
        @media(max-width: 1024px){
        display: block;}
        .btn{
            margin-top: 20px;
        }
    }
}

</style>