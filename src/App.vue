<script setup>
import TheHeader from './components/TheHeader.vue'
import { ClockIcon, ListBulletIcon, ChartBarIcon } from '@heroicons/vue/24/outline'
</script>

<template>
  <TheHeader />

  <main class="flex flex-grow flex-col">
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio modi nesciunt, odit, eius quaerat
    veniam sint voluptate maxime non totam similique possimus laboriosam! Aperiam aliquam quae
    tempore unde iure fuga vero magni doloremque. Architecto porro ducimus reiciendis quas assumenda
    voluptates quibusdam adipisci nisi, quos tempore dolor sed ab iste aliquid soluta consequatur
    hic? Quaerat, eaque itaque. Ullam illo repellat cumque similique reprehenderit amet consequatur
    labore nemo veritatis eius! Quae sit culpa provident ipsam voluptas soluta quaerat blanditiis
    excepturi eum, reiciendis adipisci beatae omnis. Doloremque quia et exercitationem ratione eius
    dolorem. Assumenda dicta corrupti eligendi aliquam, maxime iusto expedita suscipit! Eos!
  </main>

  <nav class="sticky bottom-0 z-10 bg-white">
    <ul class="flex items-center justify-around border-t">
      <li class="flex-1">
        <a
          href="#timeline"
          class="flex flex-col items-center p-2 text-xs capitalize hover:bg-gray-100"
        >
          <ClockIcon class="h-6 w-6" />
          Timeline
        </a>
      </li>
      <li class="flex-1">
        <a
          href="#activities"
          class="flex flex-col items-center p-2 text-xs capitalize hover:bg-gray-100"
        >
          <ListBulletIcon class="h-6 w-6" />
          Activities
        </a>
      </li>
      <li class="flex-1">
        <a
          href="#progress"
          class="flex flex-col items-center p-2 text-xs capitalize hover:bg-gray-100"
        >
          <ChartBarIcon class="h-6 w-6" />
          Progress
        </a>
      </li>
    </ul>
  </nav>
</template>
