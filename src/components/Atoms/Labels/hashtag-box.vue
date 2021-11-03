<template>
    <div class="hashtag-box btn" @click="copyContent">
        <span class="topword">#bestpizzaever</span>
    </div>
</template>

<script>

    export default {
        clipboard: null,
        name: "hashtag",

        methods: {

            copyContent() {


                const clipboard = require("clipboard");
                this.clipboard = new clipboard(".btn", {

                    target: function () {
                        return document.querySelector(".topword");
                    }

                })
            }
        }
    }
</script>

<style>

    .topword {
        position: absolute;
        top: 50%;
        left: 50%;
        margin-right: 50%;
        transform: translate(-50%, -50%);
        color: #ffffff;
        font-size: 45px;
        font-weight: bold;
        font-family: Alef, sans-serif;
    }

    .hashtag-box{
        width: 380px;
        height: 85px;
        background-color: #FFBA00;
        position: relative;
    }

    .hashtag-box:hover {
        cursor: pointer;
    }

    @media (max-width: 767px) {
        .hashtag-box {
            display: none;
        }
    }

</style>
