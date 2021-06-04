<template>
    <div class="welcome h-screen flex flex-col justify-around text-gray-50">
        <div>
            <h1 class=" text-6xl p-32">La basilique du Sacré Coeur</h1>
            <span class=" text-2xl p-32">Monument Historique de Paris</span>
        </div>
        <div class="flex justify-center">
            <img src="img/down-arrow.png">
        </div>
    </div>
</template>

<script>
    export default {
        name: 'welcome',
    }
</script>

<style>

    .nav[data-v-408680e8] {
        background-image: url("/img/sc.jpeg");
    }

    .welcome {
        background-image: url("/img/sc.jpeg");
        background-position: top center;
        background-size: cover;
        background-repeat: no-repeat;
        background-attachment: fixed;
    }
</style>
