<script setup>
import Card from "./Card.vue";

defineProps({
  items: Array,
});

const onClickAdd = () => {
  alert("Добавить");
};

const emit = defineEmits(["addToFavorite", "addToCart"]);
</script>

<template>
  <div class="grid grid-cols-4 gap-5">
    <Card
      v-for="item in items"
      :key="item.id"
      :id="item.id"
      :title="item.title"
      :image-url="item.imageUrl"
      :price="item.price"
      :onClickFavorite="() => emit('addToFavorite', item)"
      :isFavorite="item.isFavorite"
      :onClickAdd="() => emit('addToCart', item)"
      :isAdded="item.isAdded"
    />
  </div>
</template>
