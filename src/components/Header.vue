<template>
  <header>
    <div class="container header-menus">
        <div class="header-logo">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <div class="header-nav">
            <ul class="header-menu-nav">
                <li v-for="(link, index) in links" :key="index" :class="{'active': link.active}">
                    <a :href="link.url">{{link.text}}</a>
                </li>
               
            </ul>
        </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data: function() {
    return {
        links: [
            {
                text: 'characters',
                url: '#',
                active: false
            },
            {
                text: 'comics',
                url: '#',
                active: true
            },
            {
                text: 'movies',
                url: '#',
                active: false
            },
            {
                text: 'tv',
                url: '#',
                active: false
            },
            {
                text: 'games',
                url: '#',
                active: false
            },
            {
                text: 'collectibles',
                url: '#',
                active: false
            },
            {
                text: 'videos',
                url: '#',
                active: false
            },
            {
                text: 'fans',
                url: '#',
                active: false
            },
            {
                text: 'news',
                url: '#',
                active: false
            },
            {
                text: 'shop',
                url: '#',
                active: false
            },
        ],
    };
  }
};
</script>

<style scoped lang="scss">
    @import '../style/variables.scss';

    header{
        width: 100%;
        height: 100px;
        background-color: $brand_secondary_color;
        line-height: 100px;
        text-transform: uppercase;
        
        .header-menus{
            display: flex;

            .header-logo {
                width: 40%;
                
                img{
                    width: 60px;
                    vertical-align: middle;
                }
            }
            .header-nav {
                width: 60%;
                
                .header-menu-nav{
                    display: flex;

                    
                    
                    li{
                        font-size: 12px;
                        padding: 0 10px;

                        &.active a {
                            color: $brand_primary_color;
                            border-bottom: 5px solid $brand_primary_color;
                        }
                        a{  
                            display: inline-block;
                            line-height: 90px;

                            
                        }
                    }
                }
            }
        }

        
    }
    

</style>
