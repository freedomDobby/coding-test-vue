<script setup lang="ts">
//  반복되는 구조 component
const props = defineProps({
  numberValue: Number,
  title: String,
});
</script>

<template>
  <div class="statItem">
    <span class="statValue">{{ props.numberValue }}</span>
    <span class="statLabel">{{ props.title }}</span>
  </div>
</template>

<style scoped>
.statItem {
  display: grid;
}

.statValue {
  font-weight: 700;
  font-size: 18px;
}
.statLabel {
  color: var(--muted);
}
</style>
