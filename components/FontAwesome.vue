<script setup lang="ts">
import { PropType, computed } from 'vue';

const $props = defineProps({
  name: { type: String, required: true },
  animation: { type: String, required: false },
  variant: { type: String, required: false },
  mode: { type: String as PropType<'solid' | 'regular' | 'duotone' | 'brands'>, default: 'regular' },
})

const classes = computed(() => [
  `fa-${$props.animation}`,
  `fa-${$props.name}`,
  `fa-${$props.mode}`,
  `text-${$props.variant}`,
].join(' '))
</script>

<template>
  <span :class="classes"/>
</template>