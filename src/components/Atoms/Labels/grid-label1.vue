<template>
    <div class="grid">

        <p class="grid-item grid-item1" @click="scrollToBottom">Menu</p>

        <p class="grid-item">Regular</p>

        <p class="grid-item">Weekend</p>

        <p class="grid-item">For kids</p>

        <p class="grid-item">Delivery</p>
    </div>
</template>

<script>
    export default {
        name: "grid-label1",
        methods: {
            scrollToBottom() {
                const element = document.getElementById("footer");

                element.scrollIntoView()

            }
        }
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
        font-weight: bold;
        font-size: larger;
    }
    
    .grid-item1:hover {
        cursor:pointer;
    }

</style>