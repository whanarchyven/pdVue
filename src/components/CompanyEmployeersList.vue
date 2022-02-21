<script setup>
import { ref } from 'vue'
import CompanyEmployeerCardDemo from "./CompanyEmployeerCardDemo.vue";

defineProps({
  employers:Array,
})


</script>

<template>
  <div class="w-full relative  p-20">
    <h2 class="text-[55px] font-semibold text-black text-left mt-[55px] mb-[100px]">Сотрундники Компании</h2>
    <div class="grid cols relative grid-cols-4">
      <div v-for="(employer,index) in employers">
        <company-employeer-card-demo v-if="index<4" :employer="employer"></company-employeer-card-demo>
      </div>
      <div class="absolute h-full w-[25%] right-0 bg-gradient-to-r from-transparent to-white">
        <div class="w-[190px] bg-white cursor-pointer h-[95px] rounded-[20px] absolute right-0 top-[33%] font-proxima italic text-[24px] font-bold border-black border-2 text-right pr-[10px]">
          <p>
            Смотреть всех
          </p>
          <img class="pr-[10px] ml-auto" src="../assets/arrow_right.svg">
        </div>
      </div>
    </div>

  </div>


</template>

<style scoped>

</style>
