<template>
    <div class="padding">
        <ul>
            <li :key="index" v-for="(img,index) in images">
            <img :src="img.src" :key="index" alt=""><a href="">{{img.name}}</a>
            </li>
        </ul>

    </div>
</template>
<script>
    export default{
            name:"Section2",
            data(){
                return{
                    images:[
                        {
                            name:"DIGITAL COMICS",
                            src:"img/buy-comics-digital-comics.png"
                        },
                        {
                            name:"DC MERCHANDISE",
                            src:"img/buy-comics-merchandise.png"
                        },
                        {
                            name:"SUBSCRIPTION",
                            src:"img/buy-comics-subscriptions.png"
                        },
                        {
                            name:"COMIC SHOP LOCATION",
                            src:"img/buy-comics-shop-locator.png"
                        },
                        {
                            name:"VISA",
                            src:"img/buy-dc-power-visa.svg"
                        }
                    ]
                }
            }
    }
</script>
<style lang="scss" scoped>
        div{
            color: white;;
            display: flex;
            flex-direction: row;
            justify-content: center;
            align-items: center;
            padding: 50px 0 ;
            background-color: #0282f9;
            ul{
                display: flex;
                flex-direction:row ;

                li{
                    padding-right: 20px;
                    list-style: none;
                    display: flex;
                    align-items: center;

                    img{
                        height: 40%;
                    }

                    a{
                        text-decoration: none;
                        color: white;
                        margin-left: 10px;
                    }

                }

            }
        }
</style>
