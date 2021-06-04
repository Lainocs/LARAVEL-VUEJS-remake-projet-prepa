<template>
    <div>
        <div class="divnav block fixed top-0 w-screen z-20" id="navigation-bar">
            <button id="burger-btn">Menu Burger</button>
            <navbar/>
        </div>
        <div>
            <history-welcome/>
        </div>
        <div class="history-presentation">
            <history-presentation/>
        </div>
        <div>
            <enbas/>
        </div>
    </div>
</template>

<script>
    import Navbar from "@/Components/Inc/Navbar";
    import Enbas from "@/Components/Inc/Enbas";
    import historyWelcome from "@/Components/History/Welcome";
    import HistoryPresentation from "@/Components/History/Presentation";
    export default {
        name: 'history',
        components: {HistoryPresentation, historyWelcome, Enbas, Navbar},
    }
</script>

<style>

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
