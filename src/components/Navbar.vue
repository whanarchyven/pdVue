<script setup>
import { ref } from 'vue'

defineProps({
  msg: String
})

const count = ref(0)
</script>

<template>
  <div class="w-full h-[130px] bg-black content-center">
    <img src="../assets/logo.png" class="inline-block w-1/5 ">
    <div class="inline-flex justify-around w-4/5 h-full align-middle ">
      <a class="mt-auto cursor-pointer mb-auto text-[30px] hover:underline">Профиль</a>
      <a class="mt-auto cursor-pointer mb-auto text-[30px] hover:underline">Организации</a>
      <a class="mt-auto cursor-pointer mb-auto text-[30px] hover:underline">Сообщения</a>
      <a class="mt-auto cursor-pointer mb-auto text-[30px] hover:underline">Настройки</a>
    </div>
  </div>
</template>

<style scoped>
a {
  color: white;
}
</style>
