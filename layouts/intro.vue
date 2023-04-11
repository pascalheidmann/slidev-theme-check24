<script setup>
import SlidevFooter from "../components/footer.vue";
</script>
<template>
  <div class="h-full w-fulls">
    <div class="slidev-layout intro">
      <div class="my-auto">
        <slot/>
      </div>
    </div>
    <slidev-footer></slidev-footer>
  </div>
</template>
