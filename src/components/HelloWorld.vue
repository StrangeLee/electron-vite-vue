<script setup lang="ts">
import { ref } from 'vue'

const version = import.meta.env.VITE_VERSION


defineProps<{ msg: string }>()

const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <p style="font-size: 18.0px; font-weight: 600;"> version is {{ version }}</p>
    <button type="button" @click="count++">count is {{ count }}</button>
  </div>

</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
