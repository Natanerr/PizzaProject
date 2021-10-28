<template>
    <div class="read-more-button">
        <Mylabel msg="READ MORE"></Mylabel>
    </div>
</template>

<script>
    import Mylabel from "@/components/Atoms/Labels/Mylabel";

    export default {
        name: "read-more",
        components: {
            Mylabel
        }
    }
</script>


<style>
    .read-more-button {
        background-color: #FFBA00;
        border: white 4px solid;
        width: 250px;
        height: 50px;
        padding-left: 30px;
        padding-top: 15px;
        font-size: 30px;
        font-weight: 600;
        color: white;
    }

    .read-more-button .texting {
        margin: 0;
        font-family: 'Varela Round', sans-serif;
    }

    @media (max-width: 767px) {
        .read-more-button {
            display: none;
        }
    }

</style>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Varela+Round&display=swap');
</style>