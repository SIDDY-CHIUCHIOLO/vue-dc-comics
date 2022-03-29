<template>
    <div class="contain-cards">
        <div class="contain-img">
            <img :src="imageThumb" :alt="imageSeries">
        </div>
        <h4>{{imageSeries}}</h4>
    </div>
</template>

<script>
export default {
    name: "MainCards",
    props:['imageThumb', 'imagePrice', 'imageSeries', 'imageType']
}
</script>

<style lang="scss" scoped>
    .contain-cards{
        color:white;
        width: calc(84% / 6);
        margin:0 1%;
        margin-top: 40px;
        .contain-img{
            width: 100%;
            height: 160px;
            overflow: hidden;
            margin-bottom: 20px;
            img{
                width: 100%;    
            }
        }
    }
</style>