<template>
    <div class="divnav block fixed top-0 w-screen z-20" id="navigation-bar">
        <button id="burger-btn">Menu Burger</button>
        <navbar/>
    </div>
    <div>
        <welcome/>
    </div>
    <div>
        <presentation/>
    </div>
    <div>
        <enbas/>
    </div>
</template>

<script>
    import navbar from "@/Components/Inc/Navbar";
    import Enbas from "@/Components/Inc/Enbas";
    import Presentation from "@/Components/Presentation";
    import Welcome from "@/Components/Welcome";

    export default {
        components: {Welcome, Presentation, Enbas, navbar},
        props: {
            canLogin: Boolean,
            canRegister: Boolean,
            laravelVersion: String,
            phpVersion: String,
        }
    }

</script>

<style scoped>

    #navigation-bar {
        transition: top 1s;
    }

    #burger-btn {
        display: none;
    }

    @media screen and (max-width: 500px) {
        #burger-btn {
            display: block;
        }
    }

</style>
