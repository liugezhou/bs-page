<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <button type="button" @click="count++">count is {{ count }}</button>
  </div>
  <div class="w-full mx-auto text-[#fff] text-[14px]">
    <div class="flex flex-wrap sm:px-1">
      <div class="w-full sm:w-1/3 p-2 box pb-0 sm:px-1">
        <div class="bg-red-600 p-1">测试</div>
      </div>
      <div class="w-full sm:w-1/3 p-2 box pb-0 sm:px-1">
        <div class="bg-red-600 p-1">测试</div>
      </div>
      <div class="w-full sm:w-1/3 p-2 box pb-0 sm:px-1">
        <div class="bg-red-600 p-1">测试</div>
      </div>
      <div class="w-full sm:w-1/3 p-2 box pb-0 sm:px-1">
        <div class="bg-red-600 p-1">测试</div>
      </div>
      <div class="w-full sm:w-1/3 p-2 box pb-0 sm:px-1">
        <div class="bg-red-600 p-1">测试</div>
      </div>
    </div>
  </div>

</template>

<style scoped>

</style>
