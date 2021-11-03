<template>
    <div class="grid2">

        <p class="grid-item2 grid-item1" @click="scrollToBottom">Shef</p>

        <p class="grid-item2">BIO</p>

        <p class="grid-item2">Rewards</p>

        <p class="grid-item2">Qualification</p>

        <p class="grid-item2">Goals</p>

    </div>
</template>

<script>
    export default {
        name: "grid-label2",
        methods: {
            scrollToBottom() {
                const element = document.getElementById("footer");

                element.scrollIntoView()

            }
        }
    }
</script>

<style scoped>

    .grid2 {
        display: grid;
        color: white;
        grid-template-columns: repeat(1, 1fr);
        grid-template-rows: repeat(5,1fr);
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