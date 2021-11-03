<template>
    <div class="legend-wrapper">
        <my-label class="legend" msg="||| - Top in Menu!"></my-label>
        <my-label class="legend" msg="|| - Sale item!"></my-label>
        <my-label class="legend" msg="| - Made by chief!"></my-label>
    </div>
</template>

<script>
    import MyLabel from "@/components/Atoms/Labels/Mylabel.vue"

    export default {
        name: "Dishes-legend",
        components: {
            MyLabel
        }
    }
</script>

<style>
    .legend {
        display: inline-flex;
        margin: 0 30px 0 30px;
    }

    .legend-wrapper {
        border: aliceblue 2px solid;
        width: 1000px;
    }
    
    @media (max-width: 767px) {
        .legend-wrapper {
            display: block;
            position: relative;
            margin-left: -11%;
        }
    }

</style>