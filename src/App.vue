<template>
  <div class="app-content">
    <editor :editorText="editorText" @updateText="updateEditorText" />
    <result :editorText="editorText" />
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';
import editor from './components/editor/editor.vue';
import result from './components/result/result.vue';

const editorText = ref(`# Hello!

welcome online markdown editor
`
);

const updateEditorText = (text: string) => {
  editorText.value = text;
};
</script>

<style src="./app.scss" lang="sass"></style>