<script lang="ts" setup>
import { PanelLayout } from '@/shared'
import { UserItems, UserSelectedItems } from '@/widgets'
</script>

<template>
  <!-- <h1>UserItemsPage</h1> -->
  <PanelLayout>
    <template #top>
      <UserSelectedItems />
    </template>
    <template #bottom>
      <Suspense>
        <UserItems />
        <template #fallback> Loading... </template>
      </Suspense>
    </template>
  </PanelLayout>
</template>

<style lang="scss"></style>
