<script setup>
import { ref } from 'vue'
import CompanyEmployeerCardDemo from "./CompanyEmployeerCardDemo.vue";
import VacancyCard from "./VacancyCard.vue";

defineProps({
  vacancies:Array,
})


</script>

<template>
  <div class="w-full relative  p-20">
    <h2 class="text-[55px] font-semibold text-black text-left mt-[55px] mb-[100px]">Вакансии Компании</h2>
      <div class="w-full mb-8" v-for="(vacancy,index) in vacancies">
        <vacancy-card v-if="index<7" :vacancy="vacancy"></vacancy-card>
      </div>
    <button class="w-1/2 text-white cursor-pointer text-[30px] block ml-auto h-[70px] bg-black">Смотреть все вакансии</button>
  </div>


</template>

<style scoped>

</style>
