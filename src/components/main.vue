<template>
    <main>
        <div class="top d-flex">
            <div class="jumbotron">
                <div class="current-series">
                    <p>current series</p>
                </div>
            </div>
            <div class="container">
                <Product v-for="(card, index) in cards" :key="index" :img="card.thumb" :alt="card.series" :titolo="card.series" />
            </div>
            <div class="load-wrap">
                <div class="load-more">
                    <p>load more</p>
                </div>
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

import Product from "./Product.vue";

export default {
    name: 'Main',
    components: {
        Product,
    },
    data() { //data e' una funzione che restituisce il nostro object
        return {
            cards: [
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    price: "$19.99",
                    series: "Action Comics",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    price: "$3.99",
                    series: "American Vampire 1976",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    price: "$16.99",
                    series: "Aquaman",
                    type: "graphic novel"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    price: "$2.99",
                    series: "Batgirl",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    price: "$3.99",
                    series: "Batman",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    price: "$2.99",
                    series: "Batman Beyond",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    price: "$3.99",
                    series: "Batman/Superman",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    price: "$4.99",
                    series: "Batman/Superman Annual",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    price: "$5.99",
                    series: "Batman: The Joker War Zone",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    price: "$6.99",
                    series: "Batman: Three Jokers",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    price: "$4.99",
                    series: "Batman: White Knight Presents: Harley Quinn",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    price: "$16.99",
                    series: "Catwoman",
                    type: "graphic novel"
                }
            ]
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
        flex-direction: column;
        align-items: center;
        background-color: $cardsBg;
        .jumbotron {
            height: 400px;
            width: 100%;
            background-image: url(../assets/img/jumbotron.jpg);
            background-repeat: no-repeat;
            background-size: 100%;
            position: relative;
            .current-series {
                position: absolute;
                bottom: -15px;
                left: 15%;
                background-color: $fontColor;
                padding: 0.5em 1em;
                p {
                    text-transform: uppercase;
                    color: white
                }
            }

        };
        .container {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            padding: 2em;
                p {       
                    font-size: 1.3em;
                };
        
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
    .load-wrap {
        width: 100%;
        display: flex;
        justify-content: center;
        padding-bottom: 1em;
        .load-more {
            margin: 0 auto;
            padding: 0.5em 2.5em;
            background-color: $fontColor;
            p {
                font-size: 0.8em;
                color: white;
                text-transform: uppercase;
            }
        }
    }

</style>