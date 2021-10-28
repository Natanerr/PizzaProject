<template>
    <div class="MenuCell">

        <Mylabel class="Cum" msg="Menu" id="menu-cell1"></Mylabel>

        <Mylabel msg="Blog" id="menu-cell2"></Mylabel>

        <Mylabel msg="About Us" id="menu-cell3"></Mylabel>

        <Mylabel msg="Contacts" id="menu-cell4"></Mylabel>
    </div>
</template>

<script>

    import Mylabel from '@/components/Atoms/Labels/Mylabel.vue'

    export default {
        name: "Menu",
        components: {
            Mylabel
        }
    }
</script>

<style>
    #menu-cell1{
        display: inline-block;
        position: absolute;
        top: 10px;
        left: 40%;
    }
    #menu-cell2{
        display: inline-block;
        position: absolute;
        top: 10px;
        left: 50%;
    }
    #menu-cell3{
        display: inline-block;
        position: absolute;
        top: 10px;
        left: 58%;
    }
    #menu-cell4{
        display: inline-block;
        position: absolute;
        top: 10px;
        left: 71%;
    }

    @media (max-width: 767px) {
        #menu-cell1 {
            left: 5%;
            top: -2%;
        }

        #menu-cell2 {
            left: 25%;
            top: -2%;
        }

        #menu-cell3 {
            left: 45%;
            top: -2%
        }

        #menu-cell4 {
            left: 75%;
            top: -2%;
        }
    }


</style>