<script setup lang="ts">
const emit = defineEmits({ 'foo-bar': () => true })

emit('foo-bar')
</script>

<template>
  <button @click="emit('foo-bar')">Foo</button>
  <button @click="$emit('foo-bar')">Foo</button>
</template>
