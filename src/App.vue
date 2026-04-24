<template>
  hello
  <div class="card-container">
    <Dongju />
    <Hyoneung />
    <Hyosun />
    <Yunsang />
  </div>
</template>

<script setup>
import Dongju from '@/components/dongju.vue';
import Hyoneung from '@/components/hyoneung.vue';
import Hyosun from '@/components/hyosun.vue';
import Yunsang from '@/components/yunsang.vue';
</script>

<style scoped>
.card-container {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(2, 200px);
  gap: 20px;
  padding: 20px;
}
</style>
