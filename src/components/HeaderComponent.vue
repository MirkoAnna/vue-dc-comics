<template>

    <div class="header-container">
        <div class="align-content relative">
            <div id="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>

            <div id="links">
                <ul>
                    <li v-for="(link, index) in links" :key="index" :class="(link.current == true) ? 'active' : '' " >
                        <a :href="link.url">{{link.text}}</a>
                    </li>
                    <!-- <li><a href="#">Characters</a></li>
                    <li class="active"><a href="#">Comics</a></li>
                    <li><a href="#">Movies</a></li>
                    <li><a href="#">Tv</a></li>
                    <li><a href="#">Games</a></li>
                    <li><a href="#">Collectibles</a></li>
                    <li><a href="#">Videos</a></li>
                    <li><a href="#">Fans</a></li>
                    <li><a href="#">News</a></li>
                    <li><a href="#">Shop</a></li> -->
                </ul>
            </div>
        </div>
    </div>

</template>


<script>
export default {
    name: 'HeaderComponent',
    data() {
        return {
            links: [
                {
                    text: "characters",
                    url: "#",
                    current: false
                },
                {
                    text: "comics" ,
                    url: "#",
                    current: true
                },
                {
                    text: "movies" ,
                    url: "#",
                    current: false
                },
                {
                    text: "tv" ,
                    url: "#",
                    current: false
                },
                {
                    text: "games" ,
                    url: "#",
                    current: false
                },
                {
                    text: "collectibles" ,
                    url: "#",
                    current: false
                },
                {
                    text: "videos" ,
                    url: "#",
                    current: false
                },
                {
                    text: "fans" ,
                    url: "#",
                    current: false
                },
                {
                    text: "news" ,
                    url: "#",
                    current: false
                },
                {
                    text: "shop" ,
                    url: "#",
                    current: false
                },
            ]
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    @import "../assets/style/variables.scss";
    @import "../assets/style/general.scss";

    // Utili
    .relative {
        position: relative;
    }

    .active {
        border-bottom: 2px solid $mainBottomBackground;
    }
    // Fine Utili

    .header-container {
        width: 100%;
        height: 14vh;
        background-color: $headerBackground;
        .align-content {
            display: flex;
            align-content: center;
        }
        #logo {
            line-height: 14vh;

            img {
                width: 65%;
                vertical-align: middle;
            }
        }


        #links {
            position: absolute;
            right: 15%;
            height: 100%;

            ul {
                display: flex;
                height: 100%;

                li {
                    display: inline;
                    line-height: 14vh;
                    height: 100%;
                    margin: 0 2%;
                    text-decoration: none;
                    font-size: 65%;
                    font-weight: bold;
                    
                    a {
                        text-transform: uppercase;
                        text-decoration: none;
                        color: $footerBottomBackground;
                    }
                    &.active, 
                    &:hover {
                    border-bottom: 2px solid $mainBottomBackground;
                    color: $mainBottomBackground;
                    }
                }
            }
        }
    }

</style>