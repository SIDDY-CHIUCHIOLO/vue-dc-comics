<template>
    <div>
        <div id="contain-footer-top">
            <div class="my-container footer-top">
                <nav>
                    <div id="first-nav-left">
                        <ul>
                            <h3>DC COMICS</h3>
                            <li v-for="(element, index) in dcComics" :key="index">
                                <a href="#"> {{element.text}} </a>
                            </li>
                        </ul>
                        <ul>
                            <h3>SHOP</h3>
                            <li v-for="(element, index) in shop" :key="index">
                                <a href="#"> {{element.text}} </a>
                            </li>
                        </ul>
                    </div>
                    <ul>
                        <h3>DC</h3>
                        <li v-for="(element, index) in dc" :key="index">
                            <a href="#"> {{element.text}} </a>
                        </li>
                    </ul>
                    <ul>
                        <h3>SITES</h3>
                        <li v-for="(element, index) in sites" :key="index">
                            <a href="#"> {{element.text}}  </a>
                        </li>
                    </ul>
                </nav>
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>

        <div id="contain-footer-bottom">
            <div class="my-container footer-bottom">
                <div>
                    <span class="button">SIGN-UP NOW!</span>
                </div>
                <div id="social-footer">
                    <span id="footer-follow">FOLLOW US</span>
                    <img src="../assets/img/footer-facebook.png" alt="">
                    <img src="../assets/img/footer-twitter.png" alt="">
                    <img src="../assets/img/footer-youtube.png" alt="">
                    <img src="../assets/img/footer-pinterest.png" alt="">
                    <img src="../assets/img/footer-periscope.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "IndexFooter",
    data: function () {
        return{
            dcComics:[
                {
                text: "Characters",
                url: "#",
                },
                {
                text: "Comics",
                url: "#",
                },
                {
                text: "Movies",
                url: "#",
                },
                {
                text: "TV",
                url: "#",
                },
                {
                text: "Games",
                url: "#",
                },
                {
                text: "Videos",
                url: "#",
                },
                {
                text: "News",
                url: "#",
                },
            ],
            shop:[
                {
                text: "Shop Dc",
                url: "#",
                },
                {
                text: "Shop Dc Collectibles",
                url: "#",
                },
            ],
            dc:[
                {
                text: "Terms of Usu",
                url: "#",
                },
                {
                text: "Privacy policy (New)",
                url: "#",
                },
                {
                text: "Ad Choices",
                url: "#",
                },
                {
                text: "Advertising",
                url: "#",
                },
                {
                text: "Jobs",
                url: "#",
                },
                {
                text: "Subscriptions",
                url: "#",
                },
                {
                text: "Talent Workshops",
                url: "#",
                },
                {
                text: "CPSC Certificates",
                url: "#",
                },
                {
                text: "Ratings",
                url: "#",
                },
                {
                text: "Shop Help",
                url: "#",
                },
                {
                text: "Contact Us",
                url: "#",
                },
            ],
            sites:[
                {
                text: "DC",
                url: "#",
                },
                {
                text: "MAD Magazine",
                url: "#",
                },
                {
                text: "DC Kids",
                url: "#",
                },
                {
                text: "DC Universe",
                url: "#",
                },
                {
                text: "DC Power Visa",
                url: "#",
                }
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
    div{
        color: white;
        #contain-footer-top{
            background-image: url(../assets/img/footer-bg.jpg);
            background-repeat: no-repeat;
            background-size: cover;
            height: 400px;
            .footer-top{
                height: 100%;
                display: flex;
                justify-content: space-between;            
                nav{
                    display: flex;
                    #first-nav-left{
                        ul{
                            li{
                                list-style-type: none;
                            }
                        }
                    }
                    ul{
                        padding: 20px;
                        h3{
                            margin-bottom: 20px;
                        }
                        li{
                            list-style-type: none;
                            color: #959595;
                            line-height: 25px;
                            a{
                                color: #959595;
                                text-decoration: none;
                                font-size: 15px;
                            }
                        }
                    }
                }
            }
        }

        #contain-footer-bottom{
            background-color: #303030;
            height: 100px;
            .footer-bottom{
                height: 100%;
                display: flex;
                justify-content: space-between;
                div{
                    display: flex;
                    align-items: center;
                    .button{
                        padding: 10px;
                        border:#0282f9 solid 2px;
                    }
                }
                #social-footer{
                    width: 30%;
                    display: flex;
                    justify-content: space-around;
                    #footer-follow{
                        color:#0282f9;
                        font-weight: bold;
                    }
                }
            }
        }
    }
</style>