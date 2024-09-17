<template>
  <div class="h-full w-full">
    <div class="flex sticky h-full">
      <div class="w-2/4 bg-gray-100 h-screen">
        <div class="p-2 space-y-2 my-10">
          <div
            v-for="annotation in annotations"
            class="bg-blue-700 text-center mx-10 px-4 py-2 text-white"
          >
            {{ annotation.name }}
          </div>
        </div>

        <pre class="bg-white">
{
  "annotations": [
    {
      "page": 1,
      "type": "meterai",
      "x": 100,
      "y": 100
    }
  ]
}</pre
        >
      </div>
      <div class="w-full bg-gray-200 overflow-y-scroll">
        <div class="p-4 space-y-3 flex flex-col">
          <div v-for="page in [1, 2, 3, 4]" class="p-4 bg-white min-h-96">
            Page: {{ page }}
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const annotations = ref([
  {
    type: 'signature',
    name: 'Signature',
  },
  {
    type: 'meterai',
    name: 'Meterai',
  },
]);
</script>
