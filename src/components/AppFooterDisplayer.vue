<script>
export default {
    name: "AppFooterDisplay",
    data() {
        return {
            navList: [
                {
                    tag: "DIGITAL COMICS",
                    link: "#",
                    img: "src/assets/img/buy-comics-digital-comics.png"
                },
                {
                    tag: "DC MERCHANDISE",
                    link: "#",
                    img: "src/assets/img/buy-comics-merchandise.png"
                },
                {
                    tag: "SUBSCRIPTION",
                    link: "#",
                    img: "src/assets/img/buy-comics-subscriptions.png"
                },
                {
                    tag: "COMIC SHOP LOCATOR",
                    link: "#",
                    img: "src/assets/img/buy-comics-shop-locator.png"
                },
                {
                    tag: "DC POWER VISA",
                    link: "#",
                    img: "src/assets/img/buy-dc-power-visa.svg"
                },
            ]
        }
    }
}
</script>

<template>
    <div class="bg">
        <div class="nav container">
            <ul>
                <li v-for="item in navList">
                    <a href="item.link">
                        <div class="img">
                            <img :src="item.img" alt="">
                        </div>
                        <div>
                            {{ item.tag }}
                        </div>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>

.bg{
    background-color: #0282f9; 

    ul{
        display: flex;
        list-style: none;
        align-items: center;

        li {
            width: calc(100% / 5);
            padding: 40px 10px;

            a {
                display: flex;
                align-items: center;
                text-decoration: none;
                color: white;

                .img{
                    width: 50px;
                    margin-right: 20px;

                    img {
                        width: 100%;
                      
                    }
                }
            }
        }
    }
}
</style>