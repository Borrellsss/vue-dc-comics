<template>
    <div class="card">
        <a href="#">
            <div class="card-image">
                <img :src="cardData.thumb" :alt="cardData.series">
            </div>
            <div class="card-text">
                <h2>{{cardData.series}}</h2>
            </div>
        </a>
    </div>
</template>

<script>
export default {
    name: "CardComponent",
    props: {
        cardData: Object,
    },
    data() {
        return {

        }
    }
}
</script>

<style lang="scss" scoped>
// *IMPORTS
@import "../style/Variables.scss";

// *STYLING
.card {
    width: calc((100% / 6) - 1rem);

    &:hover {
        transform: scale(1.2);
        position: relative;
        z-index: 1000;
        transition: all 0.3s;

        a {
            box-shadow: 0 0 10px $main-color;
            position: absolute;
            left: 0;
            right: 0;

            .card-image {
                filter: brightness(40%);
                aspect-ratio: unset;
                overflow: unset;
                position: relative;
            }
            .card-text {
                width: 100%;
                position: absolute;
                top: 50%;
                left: 0;
                transform: translatey(-50%);
                text-align: center;
                transition: all 1s;

                > h2 {
                    margin-top: 0;
                }
            }
        }
    }
}
.card-image {
    aspect-ratio: 1/1;
    overflow: hidden;
}
.card-text > h2 {
    margin-top: 0.5rem;
    font-size: 0.55rem;
    text-transform: uppercase;
}
</style>
