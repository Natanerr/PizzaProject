<template>
    <div class="guide">
        <h2>{{ msg }}</h2>
        <p>{{ text }}</p>
    </div>
</template>

<script>

    export default {
        name: "guide-menu",
        props: {
            msg: String,
            text: String
        }
    }
</script>

<style>
    .guide > h2 {
        font-family: 'Prompt', sans-serif;
        font-size: 40px;
        display: inline-block;
        margin: 50px 0 0 ;
    }

    .guide > p {
        width: 350px;
        font-family: 'Prompt', sans-serif;
        font-size: 25px;
        text-align: justify;
    }
</style>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Prompt&display=swap');
</style>