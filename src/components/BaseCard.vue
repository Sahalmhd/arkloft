<script setup>
defineProps({
  title: {
    type: String,
    default: ''
  }
})
</script>

<template>
  <div class="rounded-xl border border-slate-200 bg-white shadow-sm p-6 flex flex-col gap-4">
    <div v-if="title || $slots.header" class="flex flex-col gap-2">
      <slot name="header">
        <h3 v-if="title" class="text-xl font-semibold text-slate-800">{{ title }}</h3>
      </slot>
    </div>
    <div class="text-slate-600">
      <slot />
    </div>
    <div v-if="$slots.footer" class="mt-auto pt-4 border-t border-slate-100">
      <slot name="footer" />
    </div>
  </div>
</template>
