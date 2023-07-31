<template>
    <div class="card">
      <textarea readonly class="card-content" style="white-space: pre-line;" :value="editorText"></textarea>
    </div>
  </template>
  
  <script setup lang="ts">
  import { defineProps } from 'vue';
  
  const { editorText } = defineProps(['editorText']);
  </script>
  