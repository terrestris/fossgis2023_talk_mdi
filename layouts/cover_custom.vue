<script setup lang="ts">
import { computed } from "vue";
const props = defineProps({
  class: {
    type: String,
  },
});
</script>
<template>
  <div class="slidev-layout flex custom-cover">
      <slot />
  </div>
</template>

<style scoped>
.custom-cover {
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
  .custom-cover img {
    max-height: 70% !important;
  }
</style>