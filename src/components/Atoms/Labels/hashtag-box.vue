<template>
    <div class="hashtag-box">
        <Mylabel msg="#" class="pizzeria1"></Mylabel>
        <Mylabel msg="pizzeria." class="pizzeria"></Mylabel>
    </div>
</template>

<script>
    import Mylabel from "@/components/Atoms/Labels/Mylabel.vue"

    export default {
        name: "hashtag",
        components: {
            Mylabel
        }
    }
</script>

<style>

    .hashtag-box{
        width: 380px;
        height: 85px;
        background-color: #FFBA00;
    }

    .pizzeria .texting {
        position: absolute;
        display: inline-block;
        font-size: 45px;
        font-family: Alef, sans-serif;
        font-weight: 700;
        margin: 0;
        left: 40%;
        top: 25%;
    }

    .pizzeria1 .texting {
        display: inline-block;
        position: absolute;
        font-size: 40px;
        font-family: sans-serif;
        margin: 0;
        left: 33%;
        top:40%;
    }

</style>
