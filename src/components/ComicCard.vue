<script>
    export default {
        props: ['comic']
    };
</script>

<template>
    <div class="comic-card d-flex flex-column justify-content-center align-items-center">
        <img :src="comic.thumb" :alt="comic.series" class="img-fluid" />
        <h5>{{ comic.series }}</h5>
        <p class="comic-price">{{ comic.price }}</p>
    </div>
</template>

<style scoped lang="scss">
    @use '../../style/_variables.scss' as variables;

    .comic-card {
        padding: 10px;
        text-align: center;
        cursor: pointer;
        position: relative;

        img {
            width: 100%;
            height: 200px;
            object-fit: contain;
            margin-bottom: 10px;
            transition: transform 0.3s ease;

            &:hover {
                transform: scale(1.05);
            }
        }

        h5 {
            font-size: 16px;
            font-weight: bold;
            color: variables.$title-color;
        }

        .comic-price {
            font-size: 14px;
            color: variables.$secondary-color;
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        &:hover .comic-price {
            opacity: 1;
        }
    }
</style>