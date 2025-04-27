<template>
  <div
    class="card relative z-20 flex w-[184px] flex-col items-center justify-center rounded-lg px-14 py-12"
  >
    <p class="mb-8 text-6xl font-semibold text-white">
      {{ time.toString().padStart(2, "0") }}
    </p>
    <p class="text-sm font-semibold uppercase text-white">{{ label }}</p>
  </div>
</template>

<script setup lang="ts">
interface Props {
  time: number;
  label: string;
}

defineProps<Props>();
</script>

<style scoped>
.card {
  background: #0000004d;
  box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
  backdrop-filter: blur(6.5px);
  -webkit-backdrop-filter: blur(6.5px);
  border-radius: 10px;
  border: 1px solid rgba(255, 255, 255, 0.18);
}
</style>
