<template>
    <div class="jumbotron">

    </div>
</template>

<script>
export default {
    name: "JumbotronComponent",
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
.jumbotron {
    height: $jumbotron-height;
    background-image: url("../assets/img/jumbotron.jpg");
    background-size: cover;
    background-position: top;
}
</style>