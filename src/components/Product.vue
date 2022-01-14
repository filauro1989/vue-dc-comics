<template>
    <div class="card">
        <div class="product">
            <img
                :src="img" 
                :alt="alt"
                
            >
        </div>
        <h2>{{ titolo }}</h2>
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
        flex-basis: calc((100% / 6) - 0.4em);
        h2 {
            font-size: 0.8em;
            text-transform: uppercase;
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