<template>
  <section class="footer-bottom">
    <div class="container">
        <div class="footer-sign-up-and-follow">
            <div class="footer-sign-up">
                <a class="btn" href="#">sign-up now!</a>
            </div>
            <div class="footer-follow-us">
                <h3>follow us</h3>
                <ul class="social-links">
                    <li>
                        <a href="#"><img src="../assets/img/footer-facebook.png" alt=" Facebook logo"></a>
                    </li>
                    <li>
                        <a href="#"><img src="../assets/img/footer-twitter.png" alt="Twitter logo"></a>
                    </li>
                    <li>
                        <a href="#"><img src="../assets/img/footer-youtube.png" alt="Youtube logo"></a>
                    </li>
                    <li>
                        <a href="#"><img src="../assets/img/footer-pinterest.png" alt="Pinterest logo"></a>
                    </li>
                    <li>
                        <a href="#"><img src="../assets/img/footer-periscope.png" alt="Periscope logo"></a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Footer-bottom"
};
</script>

<style scoped lang="scss">
    @import '../style/variables.scss';

    .footer-bottom{
        width: 100%;
        background-color: #303030;
        color: $brand_primary_color;

        .footer-sign-up-and-follow{
            display: flex;
            align-items: center;
            text-transform: $transform_uppercase;
            padding: 30px 0;
            .footer-sign-up,
            .footer-follow-us{
                width: 50%;
            }
            .footer-sign-up{
                .btn{
                    border: 2px solid $brand_primary_color;
                    color: $brand_secondary_color;
                }
            }
            .footer-follow-us{
                display: flex;
                justify-content: right;
                align-items: center;
                .social-links{
                    display: flex;
                    li{
                        padding: 5px;
                    }
                }
            }
        }
    }

</style>