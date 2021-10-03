<template>
    <div class="hero" :style="`background-image: url(${bgImage})`">
    </div>
</template>

<script>
export default {
    name:"Hero",
    props:["bgImage"]
}
</script>

<style lang="scss" scoped>
    .hero{
        height:400px;
        background-size: cover;
    }
</style>