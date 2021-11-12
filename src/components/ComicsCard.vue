<template>
    <div class="card">
        <div class="cover-comics">
            <img :src="image" alt="series">
            <div class="overlay">
                <h4>{{type}}</h4>
                <h5>{{price}}</h5>
            </div>
        </div>
        <h5>{{series}}</h5>

    </div>
</template>

<script>

export default {
    name: "ComicsCard",
    props: [
        "image",
        "price",
        "series",
        "type"
    ]
}
</script>

<style lang="scss">
    .card {
        width: calc(100% / 6 - 20px);

        &:hover{
            .cover-comics .overlay{
                opacity: 1;
                backdrop-filter: blur(2px);
            }
        }

        .cover-comics{
            position: relative;
            margin-bottom: 10px;

            img{
                width: 140px;
                height: 140px;
                width: 100%;
                object-fit: cover;
                object-position: top;
            }

            .overlay{
                position: absolute;
                top: 0;
                left: 0;
                right: 0;
                bottom: 0;
                opacity: 0;
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: center;
                color: white;
                background-color: rgba($color: #000000, $alpha: .4);
            }
        }

        h5 {
            margin: 0;
            color: white;
            text-transform: uppercase;
        }

        
    }
</style>