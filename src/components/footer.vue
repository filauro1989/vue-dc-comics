<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="dc-container d-flex">
                    <div class="footer-col-left d-flex j-center">
                        <div class="col">
                            <h3>dc comics</h3>
                            <ul>
                                <li>Characters</li>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>TV</li>
                                <li>Games</li>
                                <li>Videos</li>
                                <li>News</li>
                            </ul>
                            <h3>shop</h3>
                            <ul>
                                <li>Shop DC</li>
                                <li>Shop DC Collectibles</li>
                            </ul>
                        </div>
                        <div class="col">
                            <h3>DC</h3>
                            <ul>
                                <li>Terms Of Use</li>
                                <li>Privacy policy(New)</li>
                                <li>Ad Choices</li>
                                <li>Advertising</li>
                                <li>Jobs</li>
                                <li>Subscription</li>
                                <li>Talent Workshops</li>
                                <li>CPSC Certificates</li>
                                <li>Ratings</li>
                                <li>Shop Help</li>
                                <li>Contact Us</li>
                            </ul>
                        </div>
                        <div class="col">
                            <h3>Sites</h3>
                            <ul>
                                <li>DC</li>
                                <li>MAD Magazine</li>
                                <li>DC Kids</li>
                                <li>DC Universe</li>
                                <li>DC Power Visa</li>
                            </ul>
                        </div>
                        
                    </div>
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container d-flex">
                <div class="footer-bottom-sx">
                    <button>sign-up now!</button>
                </div>
                <div class="footer-bottom-dx">
                    <h2>follow us</h2>
                    <ul>
                        <li>
                            <a href="">
                                <img src="../assets/img/footer-facebook.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="">
                                <img src="../assets/img/footer-twitter.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="">
                                <img src="../assets/img/footer-youtube.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="">
                                <img src="../assets/img/footer-pinterest.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="">
                                <img src="../assets/img/footer-periscope.png" alt="">
                            </a>
                        </li>
                    </ul>
                </div>
        </div>
    </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    data() { //data e' una funzione che restituisce il nostro object
        return {
            
        }
    }, 
}


</script>

<style lang="scss" scoped>

    @import "../assets/scss/partials/_variables.scss";
    @import "../assets/scss/partials/_commons.scss";

    .footer-top {
        background-image: url(../assets/img/footer-bg.jpg);
        .container {
            background-image: url(../assets/img/dc-logo-bg.png);
            background-repeat: no-repeat;
            background-size: 35%;
            background-position-x: 80%;
            background-position-y: 50%;
        }
    }
    .footer-col-left {
        width: 40%;
        .col {
            padding: 2em 0;
            width: calc(100% / 3);
            h3 {
                color: white;
                text-transform: uppercase;
                padding: 0.5em 0;
            };
            ul {
                list-style-type: none;
                li {
                    color: #717174;
                    padding: 0.3em 0;
                    font-size: 0.8em;
                }
            }
        }
    };
    .j-center {
        justify-content: center;
    };
    .al-center {
        align-items: center;
    }
    .footer-bottom {
        background-color: #303030;
        height: 100px;
        width: 100%;
        display: flex;
        align-items: center;

        .d-flex {
            .footer-bottom-sx {
                width: 50%;
                button {
                    text-transform: uppercase;
                    border: 1px solid $fontColor;
                    background-color: #303030;
                    font-weight: bold;
                    color: white;
                    padding: 1em;
                    cursor: pointer;
                }
            }
            .footer-bottom-dx {
                display: flex;
                width: 50%;
                justify-content: end;
                h2 {
                    text-transform: uppercase;
                    display: flex;
                    align-items: center;
                    color: $fontColor;
                    padding: 0 1em;
                }
                ul {
                    display: flex;
                    li {
                        list-style-type: none;
                        padding: 0.5em;
                    }
                }
            }
        }
    }

</style>