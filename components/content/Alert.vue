<script setup lang="ts">
  import { CAlert } from '@coreui/vue'
  import '@coreui/coreui/dist/css/coreui.min.css'
</script>

<template>
  <div>
    <CAlert color="primary">
      <ContentSlot :use="$slots.default" unwrap="p" />
    </CAlert>
  </div>
</template>