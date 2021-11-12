<template>
  <header>
    <img alt="dc logo" src="../assets/dc-logo.png">
    <ul  class="navbar">
        <li v-for="(link, i) in linkNav" :key="i"><a href="">{{link.linkText}}</a></li>
    </ul>
  </header>
</template>

<script>
export default {
    name: "Header",
    data(){
        return {
            linkNav: [
                {
                    linkText: "Characters",
                    href: "#"
                },
                {
                    linkText: "Comics",
                    href: "#"
                },
                {
                    linkText: "Movies",
                    href: "#"
                },
                {
                    linkText: "TV",
                    href: "#"
                },
                {
                    linkText: "Games",
                    href: "#"
                },
                {
                    linkText: "Collectibles",
                    href: "#"
                },
                {
                    linkText: "Videos",
                    href: "#"
                },
                {
                    linkText: "Fans",
                    href: "#"
                },
                {
                    linkText: "News",
                    href: "#"
                },
                {
                    linkText: "Shop",
                    href: "#"
                },
            ]
        }
    }
}
</script>

<style lang="scss">
@import "../styles/variables";
    header {
        display: flex;
        justify-content: space-between;
        padding-top: $paddingY;
        padding-bottom: $paddingY;

        .navbar{
            display: flex;
            align-items: center;
            list-style: none;

            li{
                margin-right: 15px;

                a{
                    text-decoration: none;
                    text-transform: uppercase;
                    font-weight: bold;
                    color: black;
                    
                    &.focus{
                        color: rgb(82, 82, 255);
                        border-bottom: rgb(82, 82, 255);
                    }
                }
            }

        }
    }
</style>