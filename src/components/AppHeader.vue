<script>
export default {
    name: "AppHeader",
    data() {
        return {
            navList: [
                {
                    tag: "CHARACTERS",
                    link: "#"
                },
                {
                    tag: "COMICS",
                    link: "#"
                },
                {
                    tag: "MOVIES",
                    link: "#"
                },
                {
                    tag: "TV",
                    link: "#"
                },
                {
                    tag: "GAMES",
                    link: "#"
                },
                {
                    tag: "COLLECTIBLES",
                    link: "#"
                },
                {
                    tag: "VIDEOS",
                    link: "#"
                },
                {
                    tag: "FANS",
                    link: "#"
                },
                {
                    tag: "NEWS",
                    link: "#"
                },
                {
                    tag: "SHOP",
                    link: "#"
                }
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="src/assets/img/dc-logo.png" alt="">
            </div>
            <div class="nav">
                <ul>
                    <li v-for="item in navList">
                        <a href="item.link">{{ item.tag }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px;

    .logo {
        width: 80px;
        height: 80px;

        img {
            width: 100%;
        }

    }

    .nav {
        ul {
            display: flex;
            list-style: none;

            li {
                display: inline-block;
                padding: 15px;

                a {
                    text-decoration: none;
                    color: black;
                }
            }

        }
    }
}</style>