<script setup>
const props = defineProps({
    numberAyah:Number,
})
</script>



<template>
<p class="ayah-text">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dolorem, eum nostrum quas at est explicabo sequi pariatur in provident aut esse consequuntur recusandae quia, ipsam a saepe et, natus illo. <RouterLink to="/" class="ayah-text__number">({{ numberAyah }})</RouterLink></p>
</template>


