<template>
    <div class="nav flex justify-between font-bold" id="navigation-bar">
        <nav class="p-6">
            <ul class="main-nav flex gap-7">
                <li><a href="/" class="text-gray-50 hover:underline">Home</a></li>
                <li><a href="/history" class="text-gray-50 hover:underline">Histoire</a></li>
                <li><a href="/contact" class="text-gray-50 hover:underline">Contact</a></li>
            </ul>
        </nav>
        <div class="flex items-center">
            <inertia-link v-if="$page.props.user" href="/dashboard" class="text-gray-50 p-6 hover:underline">
                Admin Page
            </inertia-link>

            <div v-else>
                <inertia-link :href="route('login')" class="text-gray-50 p-6 hover:underline">
                    Log in
                </inertia-link>

                <inertia-link v-if="canRegister" :href="route('register')" class="text-gray-50 p-6 ml-4 text-sm text-gray-700 hover:underline">
                    Register
                </inertia-link>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'navbar',
    }

</script>

<style scoped>

    .nav {
        background-image: none;
        background-position: top center;
        background-size: cover;
        background-repeat: no-repeat;
        transition: top 0.3s;

    }

    @media screen and (max-width: 1400px) {
        .nav {
            background-image: none;
            background-color: #26538F;
        }
    }

    @media screen and (max-width: 500px){
        .nav {
            display: none;
        }
        .main-nav {
            display: block;
        }
    }
</style>
