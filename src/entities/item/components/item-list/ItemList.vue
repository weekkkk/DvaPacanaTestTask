<script lang="ts" setup>
import type { ItemType } from '../..'
import { ItemLi } from './components'

const props = defineProps<{
  items: ItemType[]
}>()
</script>

<template>
  <ul class="item_list g-4">
    <ItemLi v-for="item in items" :item="item" />
  </ul>
</template>

<style lang="scss" scoped>
.item_list {
  display: flex;
  flex-wrap: wrap;
}
</style>
