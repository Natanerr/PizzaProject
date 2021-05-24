<template>
    <div>
        <my-label class="price" msg="10$"></my-label>
        <my-label class="price" msg="14$"></my-label>
        <my-label class="price" msg="20$"></my-label>
        <my-label class="price" msg="11$"></my-label>
    </div>
</template>

<script>
    import MyLabel from "@/components/Atoms/Labels/Mylabel.vue"

    export default {
        name: "Dishes-Prices",
        components: {
            MyLabel
        }
    }
</script>

<style>
    .price .texting {
        margin-bottom: 70px;
        font-size: 40px;
    }
</style>