<template>
  <div class="bg-color">
        <Showcase />
  </div>
</template>

<script>
import Showcase from './Showcase.vue'

export default {
    name: "Main",
    components: {
        Showcase
    }
}
</script>

<style lang="scss">
@import "../styles/variables";
    .bg-color{
        background-color: #1c1c1c;
        overflow: hidden;

        h1{
            color: white;
        }
    }
</style>