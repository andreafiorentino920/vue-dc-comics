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
                            src:"../assets/buy-comics-digital-comics.png"
                        },
                        {
                            name:"DC MERCHANDISE",
                            src:"../assets/buy-comics-merchandise.png"
                        },
                        {
                            name:"SUBSCRIPTION",
                            src:"../assets/buy-comics-subscriptions.png"
                        },
                        {
                            name:"COMIC SHOP LOCATION",
                            src:"../assets/buy-comics-shop-location.png"
                        },
                        {
                            name:"DC POWER VISA",
                            src:"../assets/buy-comics-power-visa.svg"
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

                    a{
                        text-decoration: none;
                        color: white;
                    }
                }
            }
            img{
                width: 50%;
            }
        }
</style>
