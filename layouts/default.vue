<template>
  <div>
    <div class="slidev-layout default">
      <slot/>
    </div>
    <div class="slidev-current-slide-overlay">
      <span>
        <SlideCurrentNo/> / <SlidesTotal/>
      </span>
    </div>
  </div>
</template>
<style type="text/less">
.slidev-current-slide-overlay {
  display: grid;
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  justify-content: center;
  align-content: end;
  font-size: .8rem;

  & > span {
    padding: 1rem;
  }
}
</style>
<script setup>
import SlideCurrentNo from "@slidev/client/builtin/SlideCurrentNo.vue";
import SlidesTotal from "@slidev/client/builtin/SlidesTotal.vue";
</script>
