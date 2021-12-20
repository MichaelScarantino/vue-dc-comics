<template>
  <section class="footer-top">
    <div class="container">
        <div class="footer-links-and-img">
            <div class="footer-links">
                <div class="col comics-and-shop-links">
                    <div class="comics-links">
                        <h3>dc comics</h3>
                        <ul>
                            <li v-for="(link, index) in links" :key="index" v-show="link.categories === 'comics'">
                                <a href="#">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="shop-links">
                        <h3>shop</h3>
                        <ul>
                            <li v-for="(link, index) in links" :key="index" v-show="link.categories === 'shop'">
                                <a href="#">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="col dc-links">
                    <h3>dc</h3>
                    <ul>
                        <li v-for="(link, index) in links" :key="index" v-show="link.categories === 'dc'">
                            <a href="#">{{ link.text }}</a>
                        </li>
                    </ul>
                </div>
                <div class="col sites-links">
                    <h3>sites</h3>
                    <ul>
                        <li v-for="(link, index) in links" :key="index" v-show="link.categories === 'sites'">
                            <a href="#">{{ link.text }}</a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="footer-img">
            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Footer-top",
  data: function() {
    return {
        links: [
            {
                text: 'Characters',
                categories: 'comics'
            },
            {
                text: 'Comics',
                categories: 'comics'
            },
            {
                text: 'Movies',
                categories: 'comics'
            },
            {
                text: 'TV',
                categories: 'comics'
            },
            {
                text: 'Games',
                categories: 'comics'
            },
            {
                text: 'Videos',
                categories: 'comics'
            },
            {
                text: 'News',
                categories: 'comics'
            },
            {
                text: 'Shop DC',
                categories: 'shop'
            },
            {
                text: 'Shop DC Collectibles',
                categories: 'shop'
            },
            {
                text: 'Terms Of Use',
                categories: 'dc'
            },
            {
                text: 'Privacy policy (New)',
                categories: 'dc'
            },
            {
                text: 'Ad Choices',
                categories: 'dc'
            },
            {
                text: 'Jobs',
                categories: 'dc'
            },
            {
                text: 'Subscriptions',
                categories: 'dc'
            },
            {
                text: 'Talent Workshops',
                categories: 'dc'
            },
            {
                text: 'CPSC Certificates',
                categories: 'dc'
            },
            {
                text: 'Ratings',
                categories: 'dc'
            },
            {
                text: 'Shop Help',
                categories: 'dc'
            },
            {
                text: 'Contact Us',
                categories: 'dc'
            },
            {
                text: 'DC',
                categories: 'sites'
            },
            {
                text: 'MAD Magazine',
                categories: 'sites'
            },
            {
                text: 'DC Kids',
                categories: 'sites'
            },
            {
                text: 'DC Universe',
                categories: 'sites'
            },
            {
                text: 'DC Power Visa',
                categories: 'sites'
            },
        
        ]
    };
   },
};
</script>

<style scoped lang="scss">
    @import '../style/variables.scss';

    .footer-top{
        width: 100%;
        background-image: url("../assets/img/footer-bg.jpg");
        background-size: cover;
        color: white;

        .footer-links-and-img{
            display: flex;
            .footer-links,
            .footer-img{
                width: 50%;
            }
            .footer-links{
                display: flex;
                position: relative;
                padding: 30px 0;
                .col{
                    width: calc(100% / 3);
                }
                h3{
                    text-transform: $transform_uppercase;
                    padding: 10px 0;
                    font-size: 14px;
                }
                li{
                    font-size: 11px;
                    color: gray;
                    line-height: 20px;
                }
            }
            .footer-img{
                background-image: url("../assets/img/dc-logo-bg.png");
                background-size: cover;
                background-position: center;
            }
        }
    }

</style>