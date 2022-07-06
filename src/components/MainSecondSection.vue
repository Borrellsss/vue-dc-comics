<template>
<section>
    <div class="container">
        <div class="merch">
            <ul class="flex">
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                        <span>DIGITAL COMICS</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-merchandise.png" alt="">
                        <span>DC MERCHANDISE</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                        <span>SUBSCRIPTION</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                        <span>COMIC SHOP LOCATOR</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                        <span>DC POWER VISA</span>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</section>
</template>

<script>
export default {
    name: "MainSecondSection",
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
    padding: $section-padding;
    font-size: $main-font-size;
    color: #fff;
    background-color: $main-color;

    a {
        display: flex;
        align-items: center;

        img {
            margin-right: 0.5rem;
            width: auto;
            height: 2.3rem;
        }
    }
}
.merch > .flex {
    justify-content: space-evenly;
    align-items: center;

    li:last-child img {
        height: 1.5rem;
    }
}
</style>