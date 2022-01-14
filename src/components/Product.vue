<template>
    <div class="card">
        <div class="wrapper">
            <div class="product">
                <img
                    :src="img" 
                    :alt="alt"
                >
            </div>
            <h2>{{ titolo }}</h2>
        </div>
    </div>
</template>

<script>
export default {
    name:"Product",
    props: ['img', 'alt', 'titolo', 'tipo', 'prezzo'],
    data() {
        return {

        }
    }
}
</script>

<style lang="scss">
    .card {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        flex-basis: calc((100% / 6) - 0.4em);
        .wrapper {
            display: flex;
            flex-direction: column;
        };
        h2 {
            font-size: 0.5em;
            text-transform: uppercase;
            width: 150px;
        };
        .product {
            margin: 0.2em;
            height: 150px;
            width: 150px;
            overflow: hidden;
            img {
            width: 100%;
            }
        }
    }
</style>