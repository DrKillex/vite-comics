<script>
export default {
    name: "AppFooterContacts",
    data() {
        return {
            navList: [
                {
                    name: "facebook",
                    link: "#",
                    img: "src/assets/img/footer-facebook.png"
                },
                {
                    name: "twitter",
                    link: "#",
                    img: "src/assets/img/footer-twitter.png"
                },
                {
                    name: "youtube",
                    link: "#",
                    img: "src/assets/img/footer-youtube.png"
                },
                {
                    name: "pinterest",
                    link: "#",
                    img: "src/assets/img/footer-pinterest.png"
                },
                {
                    name: "periscope",
                    link: "#",
                    img: "src/assets/img/footer-periscope.png"
                },
            ]
        }
    }
}
</script>

<template>
    <div class="bg">
        <div class="container">
            <div class="btn">
                SING-UP NOW!
            </div>
            <div class="nav">
                <div>FOLLOW US</div>
                <ul>
                    <li v-for="item in navList">
                        <a href="item.link"><img :src="item.img" :alt="item.name"></a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>

.bg {
    background-color: #303030;
    
    .container {
        display: flex;
        align-items: center;
        padding: 20px 10px;
        justify-content: space-between;
        .btn{
            color: white;
            border: 1px solid #0282f9;
            padding: 10px;
        }

        .nav{
            display: flex;
            align-items: center;
            div {
                color: #0282f9;
                margin-right: 15px;
            }

            ul {
                display: flex;
                list-style: none;

                li:not(:last-child) {
                    margin-right: 10px;
                }
            }
        }
    }
    
}
</style>