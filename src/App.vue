<script setup>

import VHeader from "@/components/VHeader.vue";
import VFooter from "@/components/VFooter.vue";
import VContainer from "@/components/VContainer.vue";
import VChineseOrder from "@/components/VChinese-order.vue";
</script>

<template>
  <v-header></v-header>
  <hr>
  <div class="main-section">
    <v-container></v-container>
    <v-chinese-order></v-chinese-order>
  </div>
  <v-footer></v-footer>
</template>

<style scoped>

</style>
