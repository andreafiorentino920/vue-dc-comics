<template>
        <div class="container-card">
            <img class="card" :src="info.thumb" :alt="info.type">
            <div class="series">
                <p>{{info.series}}</p>
            </div>
            
        </div>
</template>

<script>
export default {
        name:"Card",
        props:["info"]
}
</script>

<style lang="scss">
    .container-card{
        .card{
            width: 70%;
            height: 70%;
        }
        .series{
            p{
            color: white;
        }
        }
        
    }

</style>