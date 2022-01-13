<template>
    <header>
        <div class="container text-center d-flex bg-green">
            <div class="logo-container">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <div class="nav-list">
                <ul>
                    <li>
                        <a href="">CHARACTERS</a>
                    </li>
                    <li>
                        <a href="" class="active">COMICS</a>
                    </li>
                    <li>
                        <a href="">MOVIES</a>
                    </li>
                    <li>
                        <a href="">TV</a>
                    </li>
                    <li>
                        <a href="">GAMES</a>
                    </li>
                    <li>
                        <a href="">COLLECTIBLES</a>
                    </li>
                    <li>
                        <a href="">VIDEOS</a>
                    </li>
                    <li>
                        <a href="">FANS</a>
                    </li>
                    <li>
                        <a href="">NEWS</a>
                    </li>
                    <li>
                        <a href="">SHOP</a>
                    </li>
                </ul>
            </div>
        </div>    
    </header>
</template>

<script>
export default {
    name: 'Header',
    data() { //data e' una funzione che restituisce il nostro object
        return {
            title: "Lorem Ipsum pippo",
        }
    }, 
    methods: {
        // changeActive(indexElement) {
        // this.links.forEach(
        //     (element, index) => {
        //     if (index === indexElement) {
        //         element.current = true;
        //     } else {
        //         element.current = false;
        //     }
        //     }
        // )
        // }
}
}


</script>

<style lang="scss" scoped>

    @import "../assets/scss/partials/_variables.scss";

    .d-flex {
        align-items: center;
        justify-content: space-around;
    }
    ul {
        list-style: none;
        display: flex;
        justify-content: flex-end;
        align-items: center;
            li {
                padding: 0 0.5em;
                    a {
                        display: block;
                        text-decoration: none;
                        padding: 2em 0;
                        border-bottom: 5px solid white;
                        &:hover,
                        &:active,
                        &.active {
                            color: $fontColor;
                            border-bottom: 5px solid $fontColor;
                        }
                }
            }
    }
</style>