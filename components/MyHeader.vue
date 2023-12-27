<template>
  <header class="header">
    <div class="header__container">
      <img src="@/static/logo.png" alt="ArtGallery" class="header__logo" @click="$router.push('/')">
      <nav class="header__nav">
        <ul v-if="true">
          <li class="header__search header__list-item"><img src="@/static/SearchIconWhite.svg" alt="search">Поиск</li>
          <li class="header__favorites header__list-item" @click="$router.push('/favorites')"><img
              src="@/static/HeartIcon.svg" alt="search">Избранное</li>
        </ul>
        <ul v-else>
          <li class="header__search header__list-item"><img src="@/static/SearchIconWhite.svg" alt="search"></li>
          <li class="header__favorites header__list-item" @click="$router.push('/favorites')"><img
              src="@/static/HeartIcon.svg" alt="search"></li>
        </ul>
      </nav>
    </div>
    <div>
      <!-- <search-bar v-if="!searchInNav"></search-bar> -->
    </div>
    <div class="header__bottom-row"></div>
</header></template>


<script setup lang="ts">

</script>

<style scoped>

</style>