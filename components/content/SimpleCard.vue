<script setup lang="ts">
  import { CCard, CCardHeader, CCardTitle, CCardBody } from '@coreui/vue'
  import '@coreui/coreui/dist/css/coreui.min.css'
</script>

<template>
  <CCard text-color="primary" class="mb-3 border-top-3" :class="'border-top-' + 'primary'" style="max-width: 18rem">
    <CCardHeader>Header</CCardHeader>
    <CCardBody>
      <CCardTitle text-color="primary" color="primary">card title</CCardTitle>
      <ContentSlot :use="$slots.default" unwrap="p" />
    </CCardBody>
  </CCard>
</template>
