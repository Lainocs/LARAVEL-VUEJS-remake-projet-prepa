<template>
    <div class="contact h-screen flex flex-col justify-center text-gray-50">
        <div class="contact-text text-center flex flex-col gap-24">
            <h1 class=" text-6xl">Contact</h1>
        </div>
        <div class="flex justify-center">
            <img src="img/down-arrow.png">
        </div>
    </div>
</template>

<script>


export default {
    name: 'welcomeContact',
}
</script>

<style>

.nav[data-v-408680e8] {
    background-image: url("/img/interieur-sc.jpg");
}

.nav [data-v-408680e8] {
    z-index: 2;
}

.nav[data-v-408680e8]::after {
    position: absolute;
    z-index: 1;
    content: " ";
    width: 100%;
    height: 100%;
    background-color: rgba(69, 69, 69, 0.7);
}

.contact-text {
    z-index: 2;
}

.contact {
    background-image: url("/img/interieur-sc.jpg");
    background-position: top center;
    background-size: cover;
    background-attachment: fixed;
    background-repeat: no-repeat;
}

.contact::after {
    position: absolute;
    z-index: 1;
    content: " ";
    width: 100%;
    height: 100%;
    background-color: rgba(69,69,69,0.7);
}
</style>