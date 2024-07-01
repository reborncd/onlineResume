<template>
  <div class="flex mb-4 sm:flex-row justify-between" :class="{'flex-col': isWrap}">
    <template v-if="type === 'labelText'">
      <div
        class="label min-w-16 mr-1"
        :class="[labelBold ? 'font-bold' : '', isTitle ? 'text-lg' : 'text-sm']"
        :style="`${labelWidth ? `min-width:${labelWidth}px` : ''}`"
        >{{ label }}</div>
      <div
        class="flex-1 text-left min-w-[180px]"
        :class="{ 'sm:text-right': isWrap }">
        <a
          v-if="link"
          :href="text"
          class="text-[var(--link)]"
          target="_blank"
          >{{ text }}</a>
        <template v-else>
          {{ text }}
        </template>
      </div>
    </template>
  </div>
</template>

<script setup lang="ts">
import { RowContentProps } from './types.ts'
withDefaults(defineProps<RowContentProps>(), {
  type: 'labelText',
  link: false,
  align: 'left',
  labelBold: false,
  isWrap: false,
  isTitle: false,
  labelWidth: 80
})
</script>

<style scoped></style>
