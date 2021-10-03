<template>
        <div class="container-card">
            <div class="container">
                <div class="button top">
                    <button>CURRENT SERIES</button>
                </div>
                <div class="card-container">
                    <Card :key="index" v-for="(data,index) in myJson" :info="data"/>
                </div>
                <div class="button d-flex justify-content-center">
                    <button>LOAD MORE</button>
                </div>
            </div>
        </div>
</template>
<script>
      import json from "./dc-comics.json";
      import Card from "./Card.vue"
      export default{
          components:{
              Card
          },
          data(){
              return{
                  myJson: json
              }              
          }
          
      }
</script>
<style lang="scss" scoped>
            .container-card{
                
                position: relative;
                background-color: black;
                display: flex;
                align-items: center;
                flex-direction: column;
                padding: 50px 10px;
                // padding-left: 150px;
                // padding-right: 150px;
                // padding-top: 50px;
                // padding-bottom: 50px;
                
                .top{
                    position: absolute;
                    top: -20px;
                    right: 1060px;
                    
                    button{
                        font-weight: bold;
                        font-size: 15px;
                    }
                }
                .card-container{
                display: flex;
                flex-direction: row;
                flex-wrap: wrap;
                justify-content: center;
                }
                button{
                    background-color: #0282f9;
                    padding: 10px 80px;
                    margin-bottom: 10px;
                    color: white;
                }
            }

</style>
