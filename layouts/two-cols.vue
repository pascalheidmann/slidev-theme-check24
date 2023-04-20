<script setup lang="ts">
import SlidevFooter from "../components/footer.vue";

const props = defineProps({
  class: {
    type: String,
  },
})
</script>

<template>
  <div class="h-full w-fulls">
    <div class="slidev-layout two-columns w-full h-full grid grid-cols-2">
      <div class="col-left" :class="props.class">
        <slot/>
      </div>
      <div class="col-right" :class="props.class">
        <slot name="right"/>
      </div>
    </div>
    <slidev-footer></slidev-footer>
  </div>
</template>
