<script setup>
import { ref } from 'vue'
import InputText from './components/InputText.vue'
import InputCheckbox from './components/InputCheckbox.vue'

const name = ref('')
const newsletter = ref(false)
</script>

<template>
  <div class="max-w-xl mx-auto py-12 px-6">
    <h2 class="text-2xl font-semibold">v-model in Child Examples</h2>
    <form class="mt-6">
      <div class="mt-2">
        <InputText placeholder="Name" v-model="name" />
        <div class="mt-2">Name: {{ name }}</div>
      </div>

      <div class="mt-8">
        <label class="flex items-center">
          <InputCheckbox v-model="newsletter" />
          <span class="text-sm text-gray-700 ml-2"> Email me news and offers </span>
        </label>
        <div class="mt-2">Newsletter: {{ newsletter }}</div>
      </div>
    </form>
  </div>
</template>
