<template>
    <div class="padding">
        <div class="left">
            <img src="../img/dc-logo.png" alt="Logo">
        </div>
        <div class="right">
            <ul>
                <li>
                    <a href="#">adsdsadas</a>
                </li>
                <li>
                    <a href="#">adsdas</a>
                </li>
                <li>
                    <a href="#">dsadsa</a>
                </li>
                <li>
                    <a href="#">asddsa</a>
                </li>
            </ul>
        </div>
    </div>
</template>
<script>
    export default{
            name:"Header"
    }
</script>
<style lang="scss" scoped>
        div{
            display: flex;
            align-items: center;
            flex-direction: row;

            .left{
                width: 30%;
            }
            .right{
                display: flex;
                justify-content: center;
                width: 70%;
                ul{
                    display: flex;
                    flex-direction: row;
                    list-style: none;

                    li{
                        padding: 0 15px;
                        a{
                            text-decoration: none;
                            color: black;
                        }
                    }
                }
            }
        }
</style>
