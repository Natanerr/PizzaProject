<template>
    <div class="MenuCell">
        <a class="menu Menu1" id="Menu" @click="scrollToMenu">Menu</a>
        <a class="menu Master1" id="Master" @click="scrollToMaster">Master class</a>
        <a class="menu About1" id="About" @click="scrollToAbout">About Us</a>
        <a class="menu Gallery1" id="Gallery" @click="scrollToGallery">Gallery</a>
    </div>
</template>

<script>
    export default {
        name: "Menu",
        methods: {
            scrollToMenu() {

                let menuElement = document.getElementById("fourth-section");
                let btn = document.querySelector('.Menu1');

                function handleButtonClick() {
                    menuElement.scrollIntoView({block: "center", behavior: "smooth"});
                }

                btn.addEventListener('click', handleButtonClick);

                },

            scrollToMaster() {

                let hiddenElement = document.getElementById("sixth-section");
                let btn = document.querySelector('.Master1');

                function handleButtonClick() {
                    hiddenElement.scrollIntoView({block: "center", behavior: "smooth"});
                }

                btn.addEventListener('click', handleButtonClick);
                },

            scrollToAbout() {
                let hiddenElement = document.getElementById("fifth-section");
                let btn = document.querySelector('.About1');

                function handleButtonClick() {
                    hiddenElement.scrollIntoView({block: "center", behavior: "smooth"});
                }

                btn.addEventListener('click', handleButtonClick);
            },
            scrollToGallery() {
                let hiddenElement = document.getElementById("seventh-section");
                let btn = document.querySelector('.Gallery1');

                function handleButtonClick() {
                    hiddenElement.scrollIntoView({block: "center", behavior: "smooth"});
                }

                btn.addEventListener('click', handleButtonClick);
            }
            }
        }

</script>

<style>

    .menu {
        display: inline-flex;
        font-size: 50px;
        padding: 0 0 0 35px;
        float: right;
        font-family: Alef, sans-serif;
        flex: 1;
        color: transparent;
        -webkit-text-stroke: 3px #FFBA00;
        transition: transform 0.6s;
    }

    .menu:hover {
        -ms-transform: scale(1.3);
        -webkit-transform: scale(1.3);
        transform: scale(1.3);
        cursor: pointer;
    }

    .menu:first-child {
        margin-right: 50px;
    }




</style>