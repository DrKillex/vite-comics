<script>
export default {
    name: "AppFooterNav",
    data() {
        return {
            dcComicsList: [
                {
                    tag: "Characters",
                    link: "#"
                },
                {
                    tag: "Comics",
                    link: "#"
                },
                {
                    tag: "Movies",
                    link: "#"
                },
                {
                    tag: "TV",
                    link: "#"
                },
                {
                    tag: "Games",
                    link: "#"
                },
                {
                    tag: "Videos",
                    link: "#"
                },
                {
                    tag: "News",
                    link: "#"
                }
            ],
            shopList: [
                {
                    tag: "Shop DC",
                    link: "#"
                },
                {
                    tag: "Shop DC collectibles",
                    link: "#"
                }
            ],
            dcList: [                
                {
                    tag: "Terms Of Use",
                    link: "#"
                },
                {
                    tag: "Privacy policy (New)",
                    link: "#"
                },
                {
                    tag: "Ad choises",
                    link: "#"
                },
                {
                    tag: "Advertising",
                    link: "#"
                },
                {
                    tag: "Jobs",
                    link: "#"
                },
                {
                    tag: "Subscriptions",
                    link: "#"
                },
                {
                    tag: "Talent Workshops",
                    link: "#"
                },
                {
                    tag: "CPSC Certificates",
                    link: "#"
                },
                {
                    tag: "Ratings",
                    link: "#"
                },
                {
                    tag: "Shop Help",
                    link: "#"
                },
                {
                    tag: "Contact Us",
                    link: "#"
                },               
            ],
            sitesList: [
                {
                    tag: "DC",
                    link: "#"
                },
                {
                    tag: "MAD Magazine",
                    link: "#"
                },
                {
                    tag: "DC Kids",
                    link: "#"
                },
                {
                    tag: "DC Universe",
                    link: "#"
                },
                {
                    tag: "DC Power Visa",
                    link: "#"
                }
            ]    
    }
}
}
</script>

<template>
    <div class="bg">
        <div class="container">
            <div>
                <h2>DC COMICS</h2>
                <ul>
                    <li v-for="item in dcComicsList">
                        <a :href="item.link">{{ item.tag }}</a>
                    </li>
                </ul>
                <h2>SHOP</h2>
                <ul>
                    <li v-for="item in shopList">
                        <a :href="item.link">{{ item.tag }}</a>
                    </li>
                </ul>
            </div>
            <div>
                <h2>DC</h2>
                <ul>
                    <li v-for="item in dcList">
                        <a :href="item.link">{{ item.tag }}</a>
                    </li>
                </ul>
            </div>
            <div>
                <h2>SITES</h2>
                <ul>
                    <li v-for="item in sitesList">
                        <a :href="item.link">{{ item.tag }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.bg {
    background-image: url("src/assets/img/footer-bg.jpg");
    color: white;
    .container {
        display: flex;
        padding: 80px 10px;
        div {
            margin-right: 20px;

            ul {
            list-style: none;
            padding: 20px 0;

            a {
                color: #959595;
                text-decoration: none;
            }
        }
        }
        
    }    
}
</style>