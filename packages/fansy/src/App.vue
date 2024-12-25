<template>
  <div>
    <div>{{ count }}</div>
    <button @click="onIncrease()">increase</button>
    <button @click="onSum()">sum</button>
    <fs-button>fs-button</fs-button>
  </div>
</template>

<script setup>
import { FsButton } from '@lib/ui'
import { sum } from '@lib/shared'
import { ref } from 'vue'
const a = 1

const count = ref(0)

const onIncrease = () => {
  count.value++
}

const onSum = () => {
  console.log(sum(count.value, 10))
}
</script>

<style lang="scss" scoped></style>