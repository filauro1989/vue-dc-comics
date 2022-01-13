<template>
    <main>
        <div class="top d-flex">
            <div class="container">
                <p> --> Content goes here  </p>
            </div>
        </div>
        <div class="bottom">
            <div class="container">

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
    .top {
        background-color: black;
        height: 150px;
        .container p {       
            font-size: 1.5em;
        }
    }
    .bottom {
        background-color: $fontColor;
        height: 150px;
    }

</style>