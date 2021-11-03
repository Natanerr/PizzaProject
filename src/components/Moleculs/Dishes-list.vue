<template>
    <div>
        <my-label class="dishes-title" msg="| EIUSMOD SED DO"></my-label>
        <my-label class="dishes-composition" msg="(tempor, incididunt, utas, labore, etws)"></my-label>
        <my-label class="dishes-title" msg="|| YARE-YARE DAZE"></my-label>
        <my-label class="dishes-composition" msg="(ORA, ORA, ORA, ORA, ORA)"></my-label>
        <my-label class="dishes-title" msg="||| EIUSMOD SED DO"></my-label>
        <my-label class="dishes-composition" msg="(tempor, incididunt, utas, labore, etws)"></my-label>
        <my-label class="dishes-title" msg="|| ZA WARUDO"></my-label>
        <my-label class="dishes-composition" msg="(MUDA, MUDA, MUDA, MUDA, MUDA)"></my-label>

    </div>
</template>

<script>
    import MyLabel from "@/components/Atoms/Labels/Mylabel.vue"

    export default {
        name: "Dishes-list",
        components: {
            MyLabel
        }
    }
</script>

<style>

    .dishes-title .texting {
        text-align: left;
        line-height: 0;
        margin-bottom: -5px;
        font-family: 'Varela Round', sans-serif;
        font-size: 50px;
    }

    .dishes-composition .texting {
        text-align: left;
        margin-bottom: 60px;
        font-family: 'Varela Round', sans-serif;
        font-size:40px;
    }

    @media (max-width: 767px) {
        .dishes-title .texting {
            font-weight: bold;
            font-family: Alef, sans-serif;
            font-size: 70px;
            position: relative;
            margin-left: -23%;
            margin-top: -5%;
        }

        .dishes-composition .texting {
            position: relative;
            margin-left: -23%;
            margin-bottom: 15%;
            font-size: 45px;
        }
    }
</style>