<template>
    <div>
        <h2 class="texting">{{ msg }}</h2>
    </div>
</template>

<script>
    export default {
        name: 'menu',
        props: {
            msg: String
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .texting {
        color: white;
        font-weight: 500;
        font-size: 35px;
        font-family: Alef, sans-serif;
    }

</style>