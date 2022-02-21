<script setup>
import { ref } from 'vue'

defineProps({
  vacancy: Object
})


</script>

<template>
  <div class="w-full relative  border-2 border-black p-7">
    <h2 class="text-[30px] font-medium">{{ vacancy.name }}</h2>
    <p class="text-[22px] line-through-[26px]">{{vacancy.desc}}</p>
    <p class="text-[22px] font-medium">Размещено: {{vacancy.updated_at}}</p>
    <p class="text-[22px] font-bold absolute top-3 right-3">Цена: {{vacancy.payment}} р.</p>
  </div>
</template>

<style scoped>

</style>
