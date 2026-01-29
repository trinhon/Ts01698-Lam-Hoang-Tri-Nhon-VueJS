<template>
  <div class="p-4 border rounded mb-3">
    <h3>Bài 2: Two-way Data Binding</h3>

    <input
      v-model="userInput"
      class="form-control"
      placeholder="Nhập dữ liệu"
    />

    <p class="mt-2">Giá trị bạn nhập: {{ userInput }}</p>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const userInput = ref('FPL')
</script>
