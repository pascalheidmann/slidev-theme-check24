<script setup>
import SlidevFooter from "../components/footer.vue";
</script>
<template>
  <div class="h-full w-fulls">
    <div class="slidev-layout section">
      <slot/>
    </div>
    <slidev-footer></slidev-footer>
  </div>
</template>
