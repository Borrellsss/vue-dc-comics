<template>
<section>
    <div class="container">
        content goes here!
    </div>
</section>
</template>

<script>
export default {
    name: "MainFirstSection",
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
section {
    padding: 4rem;
    color: #fff;
    background-color: $secondary-color;
}

</style>