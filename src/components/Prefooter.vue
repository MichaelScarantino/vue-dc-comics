<template>
  <section class="pre-footer">
    <div class="container">
        <div class="pre-footer-icon">
            <ul class="pre-footer-icon-menu">
                <li v-for="(icon, index) in icons" :key="index">
                    <div class="single-icon">
                        <div class="single-icon-img">
                            <img :src="require('../assets/img/' + icon.imgIcon)" alt="">
                        </div>
                        <div class="single-icon-text">
                            {{ icon.text }}
                        </div>
                    </div>
                </li>
            </ul>
        </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Prefooter",
   data: function() {
    return {
        icons: [
            {
                imgIcon: 'buy-comics-digital-comics.png',
                text: 'digital comics'
            },
            {
                imgIcon: 'buy-comics-merchandise.png',
                text: 'dc merchandise'
            },
            {
                imgIcon: 'buy-comics-subscriptions.png',
                text: 'subsctiption'
            },
            {
                imgIcon: 'buy-comics-shop-locator.png',
                text: 'comic shpo locator'
            },
            {
                imgIcon: 'buy-dc-power-visa.svg',
                text: 'dc power visa'
            },
        ]
    };
   },
};
</script>

<style scoped lang="scss">
    @import '../style/variables.scss';

    .pre-footer{
        width: 100%;
        background-color: #0182f9;
        color: white;
        font-size: 12px;
        text-transform: $transform_uppercase;

        .pre-footer-icon-menu{
            display: flex;
            justify-content: space-around;
            align-items: center;
            
           .single-icon{
               display: flex;
               align-items: center;
               padding: 40px 0;

               img{
                width: 35px;
               }
               .single-icon-text{
                   padding-left: 10px;
               }
           }
        }
    }

</style>
