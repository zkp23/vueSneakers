<script setup>
import Header from './components/Header.vue'
import CardListView from './components/CardListView.vue'
</script>

<template>
  <div class="bg-white relative w-4/5 m-auto rounded-xl shadow-xl mt-14">
    <Header />
    <div class="p-10">
      <h2 class="text-3xl font-bold mb-8">Все кроссовки</h2>
      <CardListView />
    </div>
  </div>
</template>