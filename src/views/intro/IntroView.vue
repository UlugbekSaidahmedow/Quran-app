<script setup>
import Bismillah from '../Bismillah/Bismillah.vue';
import Ayah from '@/components/card/ayah/Ayah.vue'
import randomAyahs from "@/assets/js/randomAyahs"
</script>


<template>
   <section class="intro">
    <div class="container">
        <h1 class="title">Holy Qur'an</h1>
        <Bismillah/>
        <h2 class="intro__title text-arabic">بِٱلْحَمْدُ لِلّٰهِ ٱلَّذِي خَلَقَ ٱلْإِنْسَانَ وَٱلْجَانَّ وَ ٱلسَّمٰوَاتِ وَ ٱلْأَرْضَ وَ مَا فِيهُمَا وَ مَا بَيْنَهُمَا وَ هُوَ ذُوْ ٱلْجَلَالِ وَ ٱلْإِكْرَامِ وَ هُوَ عَلَى كُلِّ شَيْءٍ قَدِيرٌ </h2>
        <p class="intro-subtitle">All praise is for Allah Who created man and jinn and the heavens and the earth and what is in them and what is between them and He is the Lord of Majesty and Bounty and He has power over everything.</p>
        <Ayah :numberAyah="randomAyahs"/>
    </div>
   </section>
</template>


