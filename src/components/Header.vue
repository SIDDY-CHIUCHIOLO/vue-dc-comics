<template>
    <div>
        <nav>
            <img src="../assets/img/dc-logo.png" alt="">
            <ul>
                <li v-for="(element, index) in headerNav" :key="index" @click="setActiveElement(index)">
                    <a :class="{active: element.active}" href="#">{{element.text}}</a>
                </li>
            </ul>
        </nav>
    </div>
</template>

<script>
export default {
    name: "IndexHeader",
    data: function () {
        return{
            headerNav:[
                {
                text: "CHARACTERS",
                url: "#",
                active: false,
                },
                {
                text: "COMICS",
                url: "#",
                active: true,
                },
                {
                text: "MOVIES",
                url: "#",
                active: false,
                },
                {
                text: "TV",
                url: "#",
                active: false,
                },
                {
                text: "GAMES",
                url: "#",
                active: false,
                },
                {
                text: "COLLECTIBLES",
                url: "#",
                active: false,
                },
                {
                text: "VIDEOS",
                url: "#",
                active: false,
                },
                {
                text: "FANS",
                url: "#",
                active: false,
                },
                {
                text: "NEWS",
                url: "#",
                active: false,
                },
                {
                text: "SHOP",
                url: "#",
                active: false,
                },
            ]
        }
    },
    methods:{
        setActiveElement(baseIndex){
            this.headerNav.forEach((element, index) =>{
                if (baseIndex === index) {
                    element.active = true;
                } else {
                    element.active = false;
                }
            });
        }
    }
}
</script>

<style lang="scss" scoped>
    div{
        nav{
            display: flex;
            justify-content: space-around;
            align-items: center;
            img{
                width: 80px;
                vertical-align: super;
                padding: 20px 0;
            }
            ul{
                display: flex;
                li{
                    list-style-type: none;
                    padding: 0 10px;
                    a{
                        text-decoration: none;
                        padding-bottom: 46px;
                        color: black;
                        &:active,
                        &.active{
                            border-bottom:#0282f9 solid 5px;
                            color: #0282f9;
                        }
                    }
                }
            }
        }
    }
</style>