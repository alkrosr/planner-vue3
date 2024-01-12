<script setup>
import TheHeader from './components/TheHeader.vue'
import { ClockIcon, ListBulletIcon, ChartBarIcon } from '@heroicons/vue/24/outline'

const navItems = ['timeline', 'activities', 'progress']

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
      <li v-for="item in navItems" :key="item" class="flex-1">
        <a
          :href="`#${item}`"
          class="flex flex-col items-center p-2 text-xs capitalize hover:bg-gray-100"
        >
          <ClockIcon v-if="item === 'timeline'" class="h-6 w-6" />
          <ListBulletIcon v-else-if="item === 'activities'" class="h-6 w-6" />
          <ChartBarIcon v-else class="h-6 w-6" />
          {{ item }}
        </a>
      </li>
    </ul>
  </nav>
</template>
