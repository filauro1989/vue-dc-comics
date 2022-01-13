<template>
    <footer>
        <div class="container">
            <div class="dc-container d-flex">
                <div class="footer-col-left d-flex j-center al-center">
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
    </footer>
</template>

<script>
export default {
    name: 'Main',
    data() { //data e' una funzione che restituisce il nostro object
        return {
            
        }
    }, 
}


</script>

<style lang="scss" scoped>

    @import "../assets/scss/partials/_variables.scss";

    footer {
        background-image: url(../assets/img/footer-bg.jpg);
        padding: 2em 0;
    }
    .footer-col-left {
        width: 40%;
        .col {
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

</style>