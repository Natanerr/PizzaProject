<template>
    <div class="grid3">

        <p class="grid-item3 grid-item1">Contact</p>

        <p class="grid-item3">Email</p>

        <p class="grid-item3">Map</p>

        <p class="grid-item3">Reception</p>

        <p class="grid-item3">Telephone</p>

    </div>
</template>

<script>
    export default {
        name: "grid-label3"
    }
</script>

<style scoped>

    .grid3 {
        display: grid;
        color: white;
        grid-template-rows: repeat(5,1fr);
        grid-template-columns: repeat(1,1fr);
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