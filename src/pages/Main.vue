<script setup lang="ts">
import Link from '../components/Link.vue'
const contactLinks = [
  {
    text: 'github',
    href: 'https://github.com/eugeneshangin',
  },
  {
    text: 'telegram',
    href: 'https://telegram.me/eugeneshangin',
  },
  {
    text: 'career',
    href: 'https://career.habr.com/eugeneshangin',
  },
  {
    text: 'linkedin',
    href: 'https://www.linkedin.com/in/%D0%B5%D0%B2%D0%B3%D0%B5%D0%BD%D0%B8%D0%B9-%D1%88%D0%B0%D0%BD%D0%B3%D0%B8%D0%BD-319727183/',
  },
]
</script>

<template>
  <div class="flex items-center justify-center h-screen
   bg-fixed bg-center bg-cover main flex-col text-white">
    <h1 class="text-4xl font-semibold">Eugene Shangin</h1>
    <div class="text-xl  mt-4">
      Frontend/fullstack developer over 8+ years
    </div>
    <div class="tracking-widest mt-4">
      Javascript Typescript Vue.js Node.js Python Postgresql
    </div>
    <div class="flex flex-wrap flex-row tracking-widest justify-center mt-4">
      <Link
          v-for="(link, index) in contactLinks"
          :key="index"
          :text="link.text"
          :href="link.href"
      />
    </div>
  </div>
</template>

<style scoped>
.main {
  background-image: linear-gradient(rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.3)),
  url('https://sun9-73.userapi.com/impf/c840122/v840122872/327c0/V1zs0pCFdH8.jpg?size=2560x1920&quality=96&sign=ed48f1146dbcbfd23ea95ad249e8e971&type=album');
}
</style>
