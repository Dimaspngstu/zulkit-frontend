<script setup>
import { ref } from 'vue'
import CategoriesCard from './../layout/CategoriesCard.vue'

const categories = ref([
    { id: 1, title: 'Mobile Ui Kit', Count:224, image: 'categories-1.jpg' },
    { id: 2, title: 'Font', Count: 751, image: 'categories-2.jpg' },
    { id: 3, title: 'Buku', Count: 100, image: 'categories-3.jpg' },
    { id: 4, title: 'Baju', Count: 441, image: 'categories-4.jpg' },
])
</script>

<template>
    <div class="container px-4 mx-auto my-16 md:px-12">
        <h2 class="mb-4 text-xl font-medium md:mb-0 md:text-lg">Top Categories</h2>
        <div class="flex flex-wrap -mx-1 lg:-mx-4">
            <CategoriesCard 
            v-for="category in categories"
            :key="category.id"
            :title="category.title"
            :Count="category.Count"
            :image="category.image"/>
        </div>
    </div>
</template>: