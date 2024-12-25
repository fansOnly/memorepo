<template>
<div class="button"><slot /></div>
</template>

<script setup>
defineOptions({
  name: 'FsButton'
})
</script>

<style lang="scss" scoped>
.button {
  padding: 8px 24px;
  background-color: #4CAF50;
  color: white;
  border-radius: 4px;
  cursor: pointer;
}
</style>