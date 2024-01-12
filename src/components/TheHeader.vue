<script setup>
import { CheckCircleIcon } from '@heroicons/vue/24/solid'
</script>

<template>
  <header class="sticky top-0 z-20 flex items-center justify-between border-b bg-white p-3">
    <a href="#">
      <div>MY PLANNER</div>
    </a>
    <a href="#" class="text-sm">
      <div v-if="true" class="flex items-center gap-1">
        <div>Progress: <span class="font-mono">33%</span></div>
        <div class="h-3 w-3 rounded-full bg-red-500"></div>
      </div>
      <div v-else class="flex items-center gap-1">
        Day complete! <CheckCircleIcon class="h-7 text-green-500" />
      </div>
    </a>
  </header>
</template>
