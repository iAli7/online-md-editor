<template>
    <div class="card">
        <textarea class="card-content" :value="editorText"></textarea>
    </div>
</template>

<style src="./editor.scss" lang="sass"></style>

<script setup lang="ts">
defineProps(['editorText'])
</script>