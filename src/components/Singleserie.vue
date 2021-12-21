<template>
    <div class="single-serie">
        <img :src="seriesObject.thumb" :alt="seriesObject.series">
        <div class="single-serie-title">
            {{ seriesObject.series }}
        </div>
    </div>
</template>

<script>
export default {
  name: "Singleserie",
  props:['seriesObject'],
};

</script>
   
<style scoped lang="scss">
    @import '../style/variables.scss';

    .single-serie{
        margin: 0 15px;
        margin-bottom: 60px;
        width: calc( (100% / 6) - 30px );
        height: 150px;
        position: relative;
        img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
        }

        .single-serie-title{
            text-transform: $transform_uppercase;
            font-size: 12px;
            padding-top: 10px;
        }
    }
</style>
