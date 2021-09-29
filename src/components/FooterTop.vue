<template>
    <div class="container">
        <div class="left-bar padding">
            <div class="col-left">
                <p>DC COMICS</p>
                <ul>
                    <li v-for="(link,index) in menu1" :key="index"><a href="">{{link.text}}</a></li>
                </ul>
                <p>SHOP</p>
                <ul>
                    <li v-for="(link,index) in menu2" :key="index"><a href="">{{link.text}}</a></li>
                </ul>
            </div>
            <div class="col-center">
                <p>DC</p>
                <ul>
                    <li v-for="(link,index) in menu3" :key="index"><a href="">{{link.text}}</a></li>
                </ul>
                
            </div>
            <div class="col-right">
                <p>SITES</p>
                <ul>
                    <li v-for="(link,index) in menu4" :key="index"><a href="">{{link.text}}</a></li>
                </ul>
            </div>
        </div>
        <div class="right-bar">
        </div>
    </div>
</template>
<script>
    export default{
            name:"FooterTop",
            data(){
                return{
                    menu1:[
                        {
                            text:"Characters",
                            url:"",
                            current:false
                        },
                        {
                            text:"Comics",
                            url:"",
                            current:false
                        },
                        {
                            text:"Movies",
                            url:"",
                            current:false
                        },
                        {
                            text:"TV",
                            url:"",
                            current:false
                        },
                        {
                            text:"Games",
                            url:"",
                            current:false
                        },
                        {
                            text:"Videos",
                            url:"",
                            current:false
                        },
                        {
                            text:"News",
                            url:"",
                            current:false
                        },
                    ],
                    menu2:[
                        {
                            text:"Shop DC",
                            url:"",
                            current:false
                        },
                        {
                            text:"Shop DC Collectibles",
                            url:"",
                            current:false
                        }
                    ],
                    menu3:[
                        {
                            text:"Term Of Use",
                            url:"",
                            current:false
                        },
                        {
                            text:"Privacy policy(New)",
                            url:"",
                            current:false
                        },
                        {
                            text:"Advertising",
                            url:"",
                            current:false
                        },
                        {
                            text:"Jobs",
                            url:"",
                            current:false
                        },
                        {
                            text:"Subscriptions",
                            url:"",
                            current:false
                        },
                        {
                            text:"Talent Workshops",
                            url:"",
                            current:false
                        },
                        {
                            text:"CPSC Certificates",
                            url:"",
                            current:false
                        },
                        {
                            text:"Ratings",
                            url:"",
                            current:false
                        },
                        {
                            text:"Shop Help",
                            url:"",
                            current:false
                        },
                        {
                            text:"GAMES",
                            url:"",
                            current:false
                        },
                        {
                            text:"Contact Us",
                            url:"",
                            current:false
                        }
                    ],
                    menu4:[
                        {
                            text:"DC",
                            url:"",
                            current:false
                        },
                        {
                            text:"MAD Magazine",
                            url:"",
                            current:false
                        },
                        {
                            text:"DC Kids",
                            url:"",
                            current:false
                        },
                        {
                            text:"DC Universe",
                            url:"",
                            current:false
                        },
                        {
                            text:"DC Power Visa",
                            url:"",
                            current:false
                        }
                    ]
                }
            }
    }
</script>
<style lang="scss" scoped>
    .container{
        display: flex;
        flex-direction: row;
        background-image: url(../assets/footer-bg.jpg);
        background-size: cover;

        .left-bar{
            display: flex;
            flex-direction: row;
            padding-top: 25px;
            
            .col-left, .col-right, .col-center{
                display: flex;
                flex-direction: column;
            }
            p{
                color: white;
                font-size: 20px;
                margin: 15px 0 15px 0;
            }
            ul{
                padding-right: 30px;
                list-style: none;

                li{
                    margin-bottom: 10px;
                }
            }
            a{
                text-decoration: none;
                color: #69687a;
            }
        }
        .right-bar{
            width: 100%;
            background-image: url(../assets/dc-logo-bg.png);
            background-size: cover;
            background-position: center;
        }
    }
</style>
