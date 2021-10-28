<template>
    <div>
        <h1>{{ msg }}</h1>

        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec imperdiet lorem ut accumsan posuere.
            Donec imperdiet lorem ut accumsan posuere. Lorem ipsum dolor sit amet, consectetur adipiscing elit. </p>
    </div>
</template>

<script>
    export default {
        name: "footer-component",
        props: {
            msg: String
        },
    }
</script>

<style scoped>

    div{
        width: 350px;
        height: auto;
        margin: 2% 5% 5% 9%;
        float: left;
        min-width: 200px;
        min-height: 1px;
        font-family: Alef, sans-serif;
    }

    h1{
        color: white;
        text-align: left;
    }

    p{
        color: white;
        text-align: left;
    }



</style>