<script setup>
import SlideCurrentNo from "@slidev/client/builtin/SlideCurrentNo.vue";
import SlidesTotal from "@slidev/client/builtin/SlidesTotal.vue";
</script>
<template>
  <div>
    <div class="slidev-layout intro">
      <div class="my-auto">
        <slot/>
      </div>
    </div>

    <div class="slidev-current-slide-overlay">
      <span>
        <SlideCurrentNo/> / <SlidesTotal/>
      </span>
    </div>
  </div>
</template>
