<template>
  <slot>
    <div class="slidev-footer">
      <p>
        <SlideCurrentNo/> / <SlidesTotal/>
      </p>
    </div>
  </slot>
</template>

<script>
import SlidesTotal from "@slidev/client/builtin/SlidesTotal.vue";
import SlideCurrentNo from "@slidev/client/builtin/SlideCurrentNo.vue";

export default {
  name: "slidev-footer",
  components: {SlideCurrentNo, SlidesTotal}
}
</script>
<style scoped>
p {
  padding: 1rem;
}

.slidev-footer {
  @apply grid h-full w-full full justify-center content-end pointer-events-none absolute bottom-0 top-0 left-0 right-0 text-xs;
}
</style>
