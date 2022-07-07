<template>
<footer>
    <!-- footer top section -->
    <div class="footer-top">
        <div class="container">
            <div class="flex">
                <div class="footer-top-left flex">
                    <div class="footer-top-left-merch">
                        <!-- dc comics -->
                        <div class="dc-comics">
                            <h4>DC COMICS</h4>
                            <ul>
                                <li>
                                    <a href="#">Charcters</a>
                                </li>
                                <li>
                                    <a href="#">Comics</a>
                                </li>
                                <li>
                                    <a href="#">Movies</a>
                                </li>
                                <li>
                                    <a href="#">TV</a>
                                </li>
                                <li>
                                    <a href="#">Games</a>
                                </li>
                                <li>
                                    <a href="#">Videos</a>
                                </li>
                                <li>
                                    <a href="#">News</a>
                                </li>
                            </ul>
                        </div>
                        <!-- shop -->
                        <div class="shop">
                            <h4>SHOP</h4>
                            <ul>
                                <li>
                                    <a href="#">Shop DC</a>
                                </li>
                                <li>
                                    <a href="#">Shop DC Collectibles</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <!-- dc -->
                    <div class="dc">
                        <h4>DC</h4>
                        <ul>
                            <li>
                                <a href="#">Terms Of Use</a>
                            </li>
                            <li>
                                <a href="#">Privacy Policy (New)</a>
                            </li>
                            <li>
                                <a href="#">Ad Choices</a>
                            </li>
                            <li>
                                <a href="#">Advertising</a>
                            </li>
                            <li>
                                <a href="#">Jobs</a>
                            </li>
                            <li>
                                <a href="#">Subscriptions</a>
                            </li>
                            <li>
                                <a href="#">Talent Workshops</a>
                            </li>
                            <li>
                                <a href="#">CPSC Certificates</a>
                            </li>
                            <li>
                                <a href="#">Ratings</a>
                            </li>
                            <li>
                                <a href="#">Shop Help</a>
                            </li>
                            <li>
                                <a href="#">Contact Us</a>
                            </li>
                        </ul>
                    </div>
                    <!-- sites -->
                    <div class="sites">
                        <h4>SITES</h4>
                        <ul>
                            <li>
                                <a href="#">DC</a>
                            </li>
                            <li>
                                <a href="#">MAD Magazine</a>
                            </li>
                            <li>
                                <a href="#">DC Kids</a>
                            </li>
                            <li>
                                <a href="#">DC Universe</a>
                            </li>
                            <li>
                                <a href="#">DC Power Visa</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="footer-top-right">
                    
                </div>
            </div>
        </div>
    </div>
    <!-- footer bottom section -->
    <div class="footer-bottom">
        <div class="container">
            <div class="flex">
                <div class="footer-bottom-left">
                    <a href="#" class="btn blue">SIGN-UP NOW!</a>
                </div>
                <div class="footer-bottom-right">
                    <div class="sites flex">
                        <span>FOLLOW US</span>
                        <div class="sites-links">
                            <ul class="flex">
                                <li>
                                    <a href="">
                                        <img src="../assets/img/footer-facebook.png" alt="facebook logo">
                                    </a>
                                </li>
                                <li>
                                    <a href="">
                                        <img src="../assets/img/footer-twitter.png" alt="twitter logo">
                                    </a>
                                </li>
                                <li>
                                    <a href="">
                                        <img src="../assets/img/footer-youtube.png" alt="youtube logo">
                                    </a>
                                </li>
                                <li>
                                    <a href="">
                                        <img src="../assets/img/footer-pinterest.png" alt="pinterest logo">
                                    </a>
                                </li>
                                <li>
                                    <a href="">
                                        <img src="../assets/img/footer-periscope.png" alt="periscope logo">
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</footer>
</template>

<script>
export default {
    name: "FooterComponent",
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
// *COMMON
h4 {
    margin-bottom: 0.5rem;
    color: #fff;
}
.footer-top,
.footer-bottom {
    .container > .flex {
        justify-content: space-between;
    }
}

// *footer top section
.footer-top {
    background: url("../assets/img/footer-bg.jpg");
}
.footer-top-left {
    padding: $footer-top-left-padding;
    width: 55%;

    &.flex {
        gap: 1.5rem;
    }

    ul {
        li {
        line-height: 0.7rem;
            a {
                font-size: $secondary-font-size;
                color: $tertiary-color;

                &:hover {
                    text-decoration: underline;
                }
            }
        }
    }
}
.footer-top-left-merch .dc-comics {
    margin-bottom: 1rem;
}
.footer-top-right {
    width: 45%;
    background: url("../assets/img/dc-logo-bg.png");
}
.footer-top,
.footer-top-right {
    background-size: cover;
    background-position: center;
}

// *footer bottom section
.footer-bottom {
    padding: $footer-bottom-padding;
    background-color: #303030;
    color: white;
}
.footer-bottom {
    .container > .flex {
        align-items: center;
    }
}
.sites {
    align-items: center;

    > span:first-of-type {
        font-size: 0.8rem;
        font-weight: $main-font-weight;
        color: $main-color;
    }
}
.sites-links li {
    margin-left: 0.8rem;
    width: $footer-bottom-sites-img-width;

    &:first-of-type {
        margin-left: 1rem;
    }
}
</style>