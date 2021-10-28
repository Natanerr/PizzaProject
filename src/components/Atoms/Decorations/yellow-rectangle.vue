<template>
    <div class="rectangle">

    </div>
</template>

<script>
    export default {
        name: "yellow-rectangle"
    }
</script>

<style scoped>
    .rectangle {
        width: 840px;
        height: 190px;
        background-color: #FFBA00;
    }

    @media (max-width: 767px) {
        .rectangle {
            display: none;
        }
    }
</style>