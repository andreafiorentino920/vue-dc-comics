<template>
    <div class="padding">
        <div class="left">
            <button>SIGN UP NOW!</button>
        </div>
        <div class="right">
            <p>FOLLOW US</p>
            <ul>
                <li :key="index" v-for="(img,index) in images">
                    <a href="#"><img :src="img.src" :key="index" alt=""></a>
                </li>
            </ul>
        </div>
    </div>
</template>
<script>
    export default{
        name:"FooterBottom",
        data(){
            return{
                 images:[
                    {
                        text:"Facebook",
                        src:"img/footer-facebook.png",
                    },
                    {
                         text:"Twitter",
                        src:"img/footer-twitter.png",
                    },
                    {
                        text:"Youtube",
                        src:"img/footer-youtube.png",
                    },
                     {
                        text:"Pinterest",
                        src:"img/footer-pinterest.png",
                    },
                    {
                        text:"Periscope",
                        src:"img/footer-periscope.png",
                    },
                   
                ]
            }
    }
}
                        
</script>
<style lang="scss" scoped>
        div{
            padding-top: 15px;
            padding-bottom: 15px;
            background-color: #303030;
            display: flex;
            align-items: center;
            flex-direction: row;

            .left{
                width: 30%;

                button{
                    border: 3px #0282f9 solid;
                    background-color: #303030;
                    color: white;
                    padding: 15px 10px
                }
            }
            .right{
                display: flex;
                justify-content: center;
                width: 70%;

                P{
                    margin-right: 5px ;
                    color: #0282f9;
                    font-weight: bold;
                } 

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