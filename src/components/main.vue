<template>
    <main>
        <div class="top d-flex">
            <div class="container">
                <p> --> Content goes here  </p>
            </div>
        </div>
        <div class="bottom d-flex">
            <div class="container d-flex space-around">
                <div class="bottom-box d-flex">
                    <div class="img-wrap">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <div class="text-wrap">
                        <p>digital comics</p>
                    </div>
                </div>
                <div class="bottom-box d-flex">
                    <div class="img-wrap">
                        <img src="../assets/img/buy-comics-merchandise.png" alt="">
                    </div>
                    <div class="text-wrap">
                        <p>digital comics</p>
                    </div>
                </div>
                <div class="bottom-box d-flex">
                    <div class="img-wrap">
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                    </div>
                    <div class="text-wrap">
                        <p>digital comics</p>
                    </div>
                </div>
                <div class="bottom-box d-flex">
                    <div class="img-wrap">
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                    </div>
                    <div class="text-wrap">
                        <p>digital comics</p>
                    </div>
                </div>
                <div class="bottom-box d-flex">
                    <div class="img-wrap">
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                    </div>
                    <div class="text-wrap">
                        <p>digital comics</p>
                    </div>
                </div>
                
            </div>
        </div>
    </main>
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
    main {
        color: white;
    }
    .d-flex {
        align-items: center;
    }
    .space-around {
        justify-content: space-around;
    }
    .top {
        background-color: black;
        height: 150px;
        .container p {       
            font-size: 1.3em;
        }
    }
    .bottom {
        background-color: $fontColor;
        height: 150px;

        .img-wrap img {
            height: 3em;
        };
        .text-wrap {
            font-size: 0.8em;
            padding: 0 1em;
            text-transform: uppercase;
        }
    }

</style>