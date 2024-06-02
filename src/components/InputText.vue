<script setup>
const props = defineProps({
  placeholder: String
})

const proxyValue = defineModel()
</script>

<template>
  <input
    type="text"
    v-model="proxyValue"
    class="rounded-md border border-gray-400 py-2 px-3 shadow-sm focus:border-indigo-500 focus:outline-none focus:ring-indigo-500 sm:text-sm placeholder:text-slate-400 mt-1 block w-full"
    :placeholder="placeholder"
  />
</template>
