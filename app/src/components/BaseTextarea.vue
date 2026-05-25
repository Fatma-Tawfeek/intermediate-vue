<template>
  <div class="form-control">
    <label class="label" :for="id">
      <span class="label-text font-medium">{{ label }}</span>
    </label>
    <textarea
      :id="id"
      class="textarea textarea-bordered w-full"
      rows="3"
      v-model="model"
      v-bind="$attrs"
    ></textarea>
  </div>
</template>

<script setup lang="ts">
defineOptions({
  inheritAttrs: false,
})

defineProps({
  id: {
    type: String,
    required: true,
  },
  label: {
    type: String,
    default: 'Description',
    required: true,
  },
})
const model = defineModel<string>()
</script>

<style scoped></style>
