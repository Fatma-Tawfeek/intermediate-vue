<template>
  <p>{{ name }}</p>
  <BaseTextInput id="name" label="Name" v-model="name" />
</template>

<script setup lang="ts">
import { ref } from 'vue'
import BaseTextInput from '@/components/BaseTextInput.vue'

const name = ref('')
</script>

<style scoped></style>
