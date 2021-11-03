<template>
    <div class="read-more-button" @click="scrollToNew">
        <Mylabel msg="READ MORE"></Mylabel>
    </div>
</template>

<script>
    import Mylabel from "@/components/Atoms/Labels/Mylabel";

    export default {
        name: "read-more",
        components: {
            Mylabel
        },
        methods: {
            scrollToNew() {
                let hiddenElement = document.getElementById("specialAnchor");
                let btn = document.querySelector('.read-more-button');

                function handleButtonClick() {
                    hiddenElement.scrollIntoView({block: "center", behavior: "smooth"});
                }

                btn.addEventListener('click', handleButtonClick);
            }
        }
    }
</script>


<style>
    .read-more-button {
        background-color: #FFBA00;
        border: white 4px solid;
        width: 250px;
        height: 50px;
        padding-top: 15px;
        font-size: 30px;
        font-weight: 600;
        color: white;
        transition: transform 0.5s;
    }

    .read-more-button:hover {
        -ms-transform: scale(1.5);
        -webkit-transform: scale(1.5);
        transform: scale(1.1);
        cursor: pointer;
    }

    .read-more-button .texting {
        margin: 0;
        font-family: 'Varela Round', sans-serif;
    }

    .read-more-button:hover {

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