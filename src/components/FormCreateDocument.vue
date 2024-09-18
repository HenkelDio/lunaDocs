<template>
  <div class="flex column q-gutter-y-md">
    <q-input
      filled
      v-model="title"
      label="Título do documento"
    />
    <q-select
      filled
      v-model="category"
      label="Categoria"
    />
    <q-input
      filled
      v-model="description"
      label="Descrição"
    />
  </div>
</template>

<script setup lang="ts">
import { watch } from 'fs';
import { ref, defineEmits } from 'vue';

const emit = defineEmits('title');
const title = ref('');
const category = ref('');
const description = ref('');

watch(title, (value) => {
  emit('title', value);
});

</script>
