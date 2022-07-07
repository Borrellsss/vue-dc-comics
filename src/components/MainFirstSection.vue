<template>
    <section>
        <div class="container">
            <div class="flex">
                <CardComponent v-for="(element, index) in comics" :key="index" :cardData="element"/>
            </div>
        </div>
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
.container > .flex {
    flex-wrap: wrap;
    gap: 1.2rem;
}
section {
    padding: $section-padding;
    color: #fff;
    background-color: $secondary-color;
}

</style>