<template>
    <section class="power-wrapper small-underline">
        <div class="container">
            <div class="row center">
                <h2 class="title">Powerfull dengan Limit PHP yang Lebih Besar</h2>
                <table class="table-power">
                    <tr>
                        <td><span class="checklist"><img alt="Vue icon" src="../assets/images/check.png"></span></td>
                        <td><p>max execution time 300s</p></td>
                    </tr>
                    <tr>
                        <td><span class="checklist"><img alt="Vue icon" src="../assets/images/check.png"></span></td>
                        <td><p>max execution time 300s</p></td>
                    </tr>
                    <tr>
                        <td><span class="checklist"><img alt="Vue icon" src="../assets/images/check.png"></span></td>
                        <td> <p>PHP memory limit 1024 MB</p> </td>
                    </tr>
                </table>


                <table class="table-power">
                    <tr>
                        <td><span class="checklist"><img alt="Vue icon" src="../assets/images/check.png"></span></td>
                        <td><p>post max size 128 MB</p></td>
                    </tr>
                    <tr>
                        <td><span class="checklist"><img alt="Vue icon" src="../assets/images/check.png"></span></td>
                        <td><p>upload max file size 128 MB</p></td>
                    </tr>
                    <tr>
                        <td><span class="checklist"><img alt="Vue icon" src="../assets/images/check.png"></span></td>
                        <td> <p>max input vars 2500</p> </td>
                    </tr>
                </table>
                <!-- <ul>
                    <li>
                        <span class="checklist"><img alt="Vue icon" src="../assets/images/check.png"></span>
                        <p>max execution time 300s</p>
                    </li>
                </ul> -->
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'PowerFull'
}
</script>
<style lang="scss">
    .center {
        text-align: center;
        margin: 0 auto;
        .table-power {
            width: 47%;
            border-collapse: collapse;
            border: 1px solid #f4f4f4;
            margin: 20px auto;
            @media(max-width: 480px){
                width: 100%;
            }
            tr {
                td {
                    border-bottom: 1px solid #f4f4f4;
                    border-top: 1px solid #f4f4f4;
                    padding: 10px 0 10px 20px;
                }
                &:nth-child(even) {
                    background: #F7F7F7;
                }
            }
        }
    }

</style>