<template>
    <div class="relative flex justify-between bg-gray-100">
        <div class="xl:w-3/5 font-bold text-2xl flex justify-center absolute mx-auto xl:-left-2/4 xl:-right-2/3 top-16 z-10">
            <div class="flex">
                <img src="/img/blue-line.png" class="w-32">
                <h2>La ville de l'amour</h2>
                <img src="/img/blue-line.png" class="w-32">
            </div>
        </div>
        <div class="presentation w-3/6 relative flex items-center">
            <img src="/img/sc.jpeg" alt="sacre-coeur" class="presentation-img xl:w-2/5 rounded-xl absolute xl:-right-20 shadow-2xl">
        </div>
        <article class="w-2/5 flex items-center p-6">
            <p class="p-10">La basilique du Sacré-Cœur de Montmartre, dite du Vœu national, située au sommet de la butte Montmartre, dans le quartier de Clignancourt du 18e arrondissement de Paris (France), est un édifice religieux parisien majeur, « sanctuaire de l'adoration eucharistique et de la miséricorde divine » et propriété de l'archidiocèse de Paris1.</p>
        </article>
    </div>
    <div class="relative flex justify-between bg-gray-100">
        <div class="xl:w-3/5 font-bold text-2xl flex justify-center absolute mx-auto xl:-left-2/3 xl:-right-2/4 top-16 z-10">
            <div class="flex">
                <img src="/img/blue-line.png" class="w-32">
                <h2>Le point culminant de Paris</h2>
                <img src="/img/blue-line.png" class="w-32">
            </div>
        </div>
        <article class="w-2/5 flex items-center p-6">
            <p class="p-10">La basilique du Sacré-Cœur de Montmartre, dite du Vœu national, située au sommet de la butte Montmartre, dans le quartier de Clignancourt du 18e arrondissement de Paris (France), est un édifice religieux parisien majeur, « sanctuaire de l'adoration eucharistique et de la miséricorde divine » et propriété de l'archidiocèse de Paris1.</p>
        </article>
        <div class="presentation w-3/6 relative flex items-center">
            <img src="/img/sc-plonge.jpeg" alt="sacre-coeur" class="presentation-img xl:w-2/5 rounded-xl absolute xl:-left-20 shadow-2xl">
        </div>
    </div>
</template>

<script>
    export default {
        name: 'presentation'
    }
</script>

<style>

    .presentation {
        background-repeat: no-repeat;
        background-size: cover;
    }

    .presentation:nth-child(2) {
        background-image: url("/img/golden-hour.jpeg");
    }
    .presentation:nth-child(3) {
        background-image: url("/img/paris-by-night.jpeg");
    }

    .presentation::after {
        content: " ";
        height: 70vh;
        width: 100vw;
        background-color: rgba(211,211,211,0.6);
    }
</style>
