<script setup>
import { RouterLink } from "vue-router";
import { Search } from "@element-plus/icons-vue";

const pages = [
  {
    path: "/",
    name: "Home",
  },
  {
    path: "/surahs",
    name: "Surahs",
  },
  {
    path: "/juzs",
    name: "Juzs",
  },
  {
    path: "/sajdas",
    name: "Sajdas",
  },
];

const search = ref("");
const menu = ref(false)
</script>

<template>
  <nav class="nav">
    <div class="nav__container">
      <div class="nav__menu" :class="{'active': menu}">
        <ul class="nav__menu-list">
          <li class="nav__menu-item" v-for="item in pages" :key="item.name">
            <RouterLink class="nav__menu-link" to="/">{{
              item.name
            }}</RouterLink>
          </li>
        </ul>
      </div>
      <form action="" class="nav__menu-form">
        <el-input
          v-model="search"
          placeholder="Please input"
          clearable
          :prefix-icon="Search"
        />
      </form>
      <RouterLink to="/" class="nav__logo text-arabic"
        >الْقُرْآن الْكَرِيْم</RouterLink
      >
      <div class="nav__burger" @click="menu = !menu">
        <div class="nav__burger-line"></div>
      </div>
    </div>
  </nav>
</template>
