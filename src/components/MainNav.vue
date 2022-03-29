<template>
    <nav id="main-nav-container">
        <div class="my-container">
            <ul>
                <li v-for="(element, index) in elementsNav" :key="index">
                    <a href="#">
                        <div>
                            <img :src="require(`@/assets/img/${element.img}`)" alt="">
                        </div>
                        <p>{{element.name}}</p>
                    </a>
                </li>
            </ul>
        </div>
    </nav>
</template>

<script>
export default {
    name:"MainNav",
    data: function(){
        return{
            elementsNav:[
                {
                    name:"DIGITAL COMICS",
                    img:"buy-comics-digital-comics.png",
                    url:"#"
                },
                                {
                    name:"DC MERCHANDISE",
                    img:"buy-comics-merchandise.png",
                    url:"#"
                },
                                {
                    name:"SUBSCRIPTION",
                    img:"buy-comics-subscriptions.png",
                    url:"#"
                },
                                {
                    name:"COMIC SHOP LOCATOR",
                    img:"buy-comics-shop-locator.png",
                    url:"#"
                },
                                {
                    name:"DC POWER VISA",
                    img:"buy-dc-power-visa.svg",
                    url:"#"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    #main-nav-container{
        background-color: #0282f9;
        height: 200px;
        .my-container{
            height: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            ul{
                display: flex;
                align-items: center;
                li{
                    list-style: none;
                    margin: 20px;
                    a{
                        text-decoration: none;
                        color: white;
                        display: flex;
                        align-items: center;
                        div{
                            width: 70px;
                            margin-right: 20px;
                            img{
                                width: 100%;
                            }
                        }
                    }
                }
            }
        }
    }
</style>