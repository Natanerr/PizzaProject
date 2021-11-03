<template>
    <div class="grid3">

        <p class="grid-item3 grid-item1" @click="scrollToBottom">Contact</p>

        <p class="grid-item3">Email</p>

        <p class="grid-item3">Map</p>

        <p class="grid-item3">Reception</p>

        <p class="grid-item3">Telephone</p>

    </div>
</template>

<script>
    export default {
        name: "grid-label3",
        methods: {
            scrollToBottom() {
                const element = document.getElementById("footer");

                element.scrollIntoView()

            }
        }
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
        font-weight: bold;
        font-size: larger;
    }

    .grid-item1:hover {
        cursor:pointer;
    }

</style>