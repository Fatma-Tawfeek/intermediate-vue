<template>
  <BaseTextInput id="name" label="Name" v-model="name" placeholder="enter name" />
  <BaseTextarea
    id="description"
    label="Description"
    v-model="description"
    placeholder="enter description"
  />
</template>

<script setup lang="ts">
import { ref } from 'vue'
import BaseTextInput from '@/components/BaseTextInput.vue'
import BaseTextarea from '@/components/BaseTextarea.vue'

const name = ref('')
const description = ref('')
</script>

<style scoped></style>
