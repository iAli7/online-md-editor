<template>
    <div class="card">
      <div class="card-content">
        {{ editorText }}
      </div>
    </div>
  </template>
  
  <script setup lang="ts">
  import { defineProps } from 'vue';
  
  const { editorText } = defineProps(['editorText']);
  </script>
  