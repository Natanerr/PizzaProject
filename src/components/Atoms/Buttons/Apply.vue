<template>
    <div class="ApplyButton">
        <my-label class="ApplyWord" msg="APPLY"></my-label>
    </div>
</template>

<script>
    import MyLabel from "@/components/Atoms/Labels/Mylabel.vue"

    export default {
        name: "Apply",
        components: {
            MyLabel
        }
    }
</script>

<style>
    .ApplyButton {
        width: 470px;
        height: 115px;
        background-color: #FFBA00;
        text-align: left;
    }

    .ApplyWord .texting {
        margin: 25px 0 0 50px;
        font-size: 45px;
        font-weight: 600;
    }

</style>