<template>
  <div class="flex w-100 items-center flex-col">
    <h1 class="text-3xl font-bold underline my-10">
      Simple Counter Application
    </h1>

    <div class="w-25 my-10">
      <Button class="w-25" label="Increase" @click="increase"/>
    </div>

    <p class="text-black">{{ count }}</p>
  </div>
</template>

<script setup>
import { ref } from 'vue'
let count = ref(0)

const increase = () => {
  count.value++
  console.log(count)
}
</script>