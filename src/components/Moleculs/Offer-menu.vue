<template>
    <div class="second-text">
        <Mylabel id="firstLi" class="offer-menu first" msg="| Sed do eiusmod tempor incididunt ut Labore et"></Mylabel>
        <Mylabel class="offer-menu second" msg="| NON-TERRAE PLUS ULTRA!"></Mylabel>
        <Mylabel class="offer-menu third " msg="| Why so slow?Break a leg or something?"></Mylabel>
    </div>
</template>

<script>
    import Mylabel from "@/components/Atoms/Labels/Mylabel.vue"

    export default {
        name: "second-section-text",
        components: {
            Mylabel
        }
    }
</script>

<style>
    .second-text .texting {
        color: white;
        font-size: 35px;
        margin: 0;
        padding: 0;
        display: flex;
        line-height: 1.5;
        font-family: Alef, sans-serif;
    }

    .first {
        position: absolute;
        top: 35%;
        left: 19%;
        margin: 0;
        padding: 0;
    }

    .second {
        position: absolute;
        top: 57%;
        left: 19%;
        margin: 0;
        padding: 0;
    }

    .third {
        position: absolute;
        top:70%;
        left:19%;
        margin: 0;
        padding: 0;
    }

    #firstLi {
        width: 680px;
        text-align: left;
        line-height: normal;
    }
    
    @media (max-width: 767px) {
        .offer-menu {
            left: 5%;
        }
        
    }
</style>