<script setup lang="ts">
defineOptions({
  name: 'IndexPage',
})
</script>

<template>
  <div>
    Minesweeper

    <div v-for="y in 10" :key="y">
      <button v-for="x in 10" :key="x" h-8 w-8 border>
        {{ (y - 1) * 10 + x }}
      </button>
    </div>
  </div>
</template>

<route lang="yaml">
meta:
  layout: home
</route>
