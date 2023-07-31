<template>
  <editor :editorText="editorText" @updateText="updateEditorText" />
  <result :editorText="editorText" />
</template>

<script setup lang="ts">
import { ref } from 'vue';
import editor from './components/editor/editor.vue';
import result from './components/result/result.vue';

const editorText = ref('');

const updateEditorText = (text: string) => {
  editorText.value = text;
};
</script>
