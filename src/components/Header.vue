<template>
    <div class="padding">
        <div class="left">
            <img src="../assets/dc-logo.png" alt="Logo">
        </div>
        <div class="right">
            <ul>
                <li v-for="(link,index) in menu" :key="index"><a href="">{{link.text}}</a></li>
            </ul>
        </div>
    </div>
</template>
<script>
    export default{
            name:"Header",
            data(){
                return{
                    menu:[
                        {
                            text:"CHARACTERS",
                            url:"",
                            current:false
                        },
                        {
                            text:"COMICS",
                            url:"",
                            current:false
                        },
                        {
                            text:"MOVIES",
                            url:"",
                            current:false
                        },
                        {
                            text:"TV",
                            url:"",
                            current:false
                        },
                        {
                            text:"GAMES",
                            url:"",
                            current:false
                        },
                        {
                            text:"COLLECTIBLES",
                            url:"",
                            current:false
                        },
                        {
                            text:"VIDEOS",
                            url:"",
                            current:false
                        },
                        {
                            text:"FANS",
                            url:"",
                            current:false
                        },
                        {
                            text:"NEWS",
                            url:"",
                            current:false
                        },
                        {
                            text:"SHOP",
                            url:"",
                            current:false
                        }

                    ]
                }
            }
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
