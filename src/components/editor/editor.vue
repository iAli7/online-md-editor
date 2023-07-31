<template>
    <div class="card">
      <textarea class="card-content" v-model="localEditorText" @input="onInputChange" />
    </div>
  </template>
  
  <script setup lang="ts">
  import { ref } from 'vue';
  
  const { editorText } = defineProps(['editorText']);
  const emit = defineEmits(['updateText']);
  
  const localEditorText = ref(editorText);
  
  const onInputChange = () => {
    emit('updateText', localEditorText.value);
  };
  </script>
  
  <style src="./editor.scss" lang="sass"></style>
  