<script setup lang="ts">
  import SBLinkButtonV3 from '@/components/SBLinkButtonV3.vue';
</script>

<template>
  <main> 
    <h2>Test, see component "SBLinkButtonV3":</h2>
    <SBLinkButtonV3 :buttonData="{ text: 'Go to start page', link : '/', targetBlank: false }"/>
  </main>
</template>
