<template>
  <header>
    <img alt="dc logo" src="../assets/dc-logo.png">
    <ul  class="navbar">
        <li><a href="">Characters</a></li>
        <li><a href="">Comics</a></li>
        <li><a href="">Movies</a></li>
        <li><a href="">Tv</a></li>
        <li><a href="">Games</a></li>
        <li><a href="">Collectibles</a></li>
        <li><a href="">Videos</a></li>
        <li><a href="">Fans</a></li>
        <li><a href="">News</a></li>
        <li><a href="">Shop</a></li>
    </ul>
  </header>
</template>

<script>
export default {
    name: "Header"
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