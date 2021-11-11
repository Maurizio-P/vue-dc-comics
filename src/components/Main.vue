<template>
  <div class="bg-color">
      <div class="container">
          <h1>--->Contents goes here  </h1>
      </div>
  </div>
</template>

<script>
export default {
    name: "Main"
}
</script>

<style lang="scss">
@import "../styles/variables";
    .bg-color{
        background-color: black;
        padding: ($paddingY * 2) 0 ;

        h1{
            color: white;
        }
    }
</style>