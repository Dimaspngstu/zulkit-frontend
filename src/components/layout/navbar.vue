<script setup>
import { RouterLink } from 'vue-router'
import Logo from './logo.vue'
import NavigationLinks from './NavigationLinks.vue'
import UserInfo from './userinfo.vue'
</script>

<template>
    <nav class="bg-white border-gray-200 px-2 sm:px-4 py-2.5 rounded dark:bg-gray-800">
        <div class="container flex flex-wrap items-center justify-between mx-auto my-2">
<Logo />
            <div class="md:order-2">
                <RouterLink to="/login"
                    class="px-8 py-3 mt-2 mr-2 text-base font-medium text-black bg-gray-200 border border-transparent rounded-full hover:bg-gray-300 md:py-2 md:text-sm md:px-8 hover:shadow">
                    Sign In
                </RouterLink>
                <a href="register.html"
                    class="px-8 py-3 text-base font-medium text-white border border-transparent rounded-full bg-navy hover:bg-navy md:py-2 md:text-sm md:px-8 hover:shadow">
                    Sign Up
                </a>
            </div>
            <UserInfo />
            <NavigationLinks />
        </div>
    </nav>
</template>