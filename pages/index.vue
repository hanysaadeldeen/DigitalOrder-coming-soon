<template>
  <div class="relative overflow-hidden">
    <ComingSoon />
    <div class="blob purple one bg-[#af99ff] opacity-40"></div>
    <div
      class="blob yellow two block bg-[#fff422] opacity-20 max-md:hidden"
    ></div>
    <div
      class="blob purple three block bg-[#af99ff] opacity-40 max-md:hidden"
    ></div>
    <div
      class="blob yellow four block bg-[#fff422] opacity-20 max-md:hidden"
    ></div>
    <div class="blob yellow five bg-[#fff422] opacity-20"></div>
  </div>
</template>

<script setup lang="ts"></script>

<style scoped>
.blob {
  position: absolute;
  width: 300px;
  height: 300px;
  border-radius: 50%;
  filter: blur(100px);
}

.one {
  top: 2%;
  left: 2%;
}

.two {
  top: 2%;
  right: 2%;
}

.three {
  bottom: 2%;

  right: 2%;
}

.four {
  bottom: 2%;
  left: 2%;
}

.five {
  top: 60%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 1000px;
  height: 300px;
}
</style>
