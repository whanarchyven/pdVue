<script setup>
import { ref } from 'vue'

defineProps({
  company: Object
})


</script>

<template>
  <div class="w-full  p-20">
    <h2 class="text-[55px] font-semibold text-black text-left mt-[55px] mb-[100px]">Компания {{company.full_name}}</h2>
    <div>
      <img src="../assets/mospolytech.jpg" class="w-4/12 inline-block">
      <div class="w-8/12 inline-block pl-[40px] align-top" >
        <div class="flow-root  w-full pb-[10px]">
          <h2 class="flow-root text-black text-left text-[35px] font-semibold">{{company.name}}</h2>
          <div class="inline-block float-left">
            <div v-for="n in 5" :key="n" class="inline-block pr-[5px]">
              <img v-if="company.rating >n" src="../assets/star_active.svg" class="w-[37px] h-[37px]">
              <img v-else src="../assets/star_passive.svg" class="w-[37px] h-[37px]">
            </div>
          </div>
          <div class="inline-block text-[24px] float-left align-middle ml-[20px]">{{company.rating}}/5</div>
          <a class="text-black cursor-pointer italic text-[24px] float-left ml-[20px] font-semibold underline">{{company.comments_quantity}} отзывов</a>
        </div>
        <h2 class="flow-root float-left text-[35px] font-medium w-full">Информация: </h2>
        <h3 class="flow-root float-left text-[24px] font-normal w-full">{{company.desc}}</h3>


      </div>
    </div>
  </div>
</template>

<style scoped>

</style>
