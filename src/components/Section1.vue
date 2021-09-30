<template>
        <div class="container">
            <Card :key="index" v-for="(data,index) in myJson" :info="data"/>
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
        div{
            background-color: black;

            .container{
                padding-left: 150px;
                display: flex;
                flex-direction: row;
                flex-wrap: wrap;
                justify-content: center;
            }
            }
</style>
