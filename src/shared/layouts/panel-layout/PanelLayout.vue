<script lang="ts" setup></script>

<template>
  <div class="panel_layout f fd-col">
    <section class="panel_layout-section-top">
      <slot name="top" />
    </section>
    <section class="panel_layout-section-bottom">
      <slot name="bottom" />
    </section>
  </div>
</template>

<style lang="scss" scoped>
.panel_layout {
  &-section {
    &-bottom {
      flex-grow: 1;
    }
  }
}
</style>
