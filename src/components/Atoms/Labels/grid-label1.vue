<template>
    <div class="grid">

        <p class="grid-item grid-item1">Menu</p>

        <p class="grid-item">Regular</p>

        <p class="grid-item">Weekend</p>

        <p class="grid-item">For kids</p>

        <p class="grid-item">Delivery</p>
    </div>
</template>

<script>
    export default {
        name: "grid-label1"
    }
</script>

<style scoped>

    .grid {
        display: grid;
        color: white;
        grid-template-columns: repeat(1, 1fr);
        grid-template-rows: repeat(5, 1fr);
        max-width: 100px;
        margin: 0 100px 0 100px;
        float: right;
        font-family: Alef, sans-serif;
    }

    .grid-item1 {
        font-style: italic;
        font-weight: bold;
        font-size: larger;
    }

</style>