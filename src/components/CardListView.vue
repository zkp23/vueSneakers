<script setup>
import Card from './Card.vue'

const onClickAdd =() => {
  alert('Добавить');
}
</script>

<template>
  <div class="grid grid-cols-4 gap-5">
    <Card title="Мужские кроссовки Nike Blazer mid Sue" 
    image-url="/sneakers/sneakers-1.jpg" 
    :price="5000" 
    :is-favorite="false"
    :on-click-add="onClickAdd"
    />
 
  </div>
</template>
