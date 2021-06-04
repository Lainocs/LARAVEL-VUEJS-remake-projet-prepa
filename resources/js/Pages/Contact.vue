<template>
    <div class="divnav block fixed top-0 w-screen z-20" id="navigation-bar">
        <button id="burger-btn">Menu Burger</button>
        <navbar/>
    </div>
    <div>
        <welcome-contact/>
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
import welcomeContact from "@/Components/Contact/Welcome.vue";

export default {
    components : {welcomeContact, Enbas, navbar}
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
