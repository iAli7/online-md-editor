<template>
  <div class="card">
    <div class="card-content" v-html="parsedMarkdown"></div>
  </div>
</template>
  
<script setup lang="ts">
import { computed } from 'vue';
import { marked } from 'marked';

const props = defineProps(['editorText']);

const parsedMarkdown = computed(() => marked(props.editorText));
</script>
