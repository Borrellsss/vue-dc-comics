<template>
    <section>
        <span class="series">CURRENT SERIES</span>
        <div class="container">
            <div class="flex">
                <CardComponent v-for="(element, index) in comics" :key="index" :cardData="element"/>
            </div>
        </div>
        <a href="#" class="btn full-blue">LOAD MORE</a>
    </section>
</template>

<script>
// *IMPORTS
import ComicsData from '../data/dc-comics.json'
import CardComponent from './CardComponent.vue'

export default {
    name: "MainFirstSection",
    components: {
        CardComponent,
    },
    data() {
        return {
            comics: ComicsData,
        }
    }
}
</script>

<style lang="scss" scoped>
// *IMPORTS
@import "../style/Variables.scss";

// *STYLING
.container {

    > .flex {
        flex-wrap: wrap;
        gap: 1.2rem;
    }
}
section {
    padding: $first-section-padding;
    color: #fff;
    background-color: $secondary-color;
    position: relative;

    .series {
        padding: 0.5rem 1rem;
        display: inline-block;
        background-color: $main-color;
        position: absolute;
        left: 17.5%;
        top: 0;
        transform: translatey(-50%);
    }
    .full-blue {
        position: absolute;
        bottom: 0;
        left: 50%;
        transform: translate(-50%, -50%);
    }
}
</style>