<template>
  <button
    class="bg-indigo-500 rounded px-2 py-1 font-bold text-white hover:bg-indigo-600"
  >
    {{ label }}
  </button>
</template>

<script setup>
defineProps({
  label: {
    type: String,
    required: true,
    default: "Click Me ",
  },
});
</script>
