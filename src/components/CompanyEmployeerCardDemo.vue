<script setup>
import { ref } from 'vue'

defineProps({
  employer: Object
})


</script>

<template>
  <div class="w-10/12  border-2 border-black rounded-[30px] p-7">
    <img src="../assets/Michael%20Wager.png" class="w-full rounded-full">
    <h3 class="font-semibold italic text-black text-[25px]">{{employer.name}}</h3>
    <p class="font-proxima italic text-[18px]">{{employer.job}}</p>
    <div>
      <img class="inline-block w-[17px]" src="../assets/email-icon.svg">
      <p class="inline-block font-proxima italic text-[15px] ml-[5px]">{{employer.email}}</p>
    </div>
    <div>
      <img class="inline-block w-[17px]" src="../assets/phone-icon.svg">
      <p class="inline-block font-proxima italic text-[15px] ml-[5px]">{{employer.phone}}</p>
    </div>
  </div>
</template>

<style scoped>

</style>
