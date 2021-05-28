<template>
    <div class="Concept-link-wrapper">
        <my-label class="Concept-link" msg="Pizza"></my-label>

        <my-label class="Concept-link" msg="Modern concept"></my-label>

        <my-label class="Concept-link" msg="Story from chief"></my-label>

        <my-label class="Concept-link" msg="Gallery"></my-label>
    </div>
</template>

<script>
    import MyLabel from "@/components/Atoms/Labels/Mylabel.vue"

    export default {
        name: "About-concept",
        components: {
            MyLabel
        }
    }
</script>

<style>
    .Concept-link .texting {
        font-size: 15px;
        margin: 0 20px;
    }

    .Concept-link-wrapper {
        display: flex;
        margin: 0;
    }

</style>