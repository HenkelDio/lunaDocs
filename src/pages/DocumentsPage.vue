<template>
  <q-page class="q-pa-lg">
    <div class="q-mb-lg flex justify-between">
      <div class="flex items-center q-gutter-x-sm">
        <div class="text-h4 text-weight-bold margin-none">Meus documentos</div>
        <q-btn icon="filter_list" flat size=".8rem" rounded style="margin-top: 4px;" />
      </div>
      <q-btn
        color="primary"
        rounded
        icon="add"
        label="Criar novo documento"
        @click="$router.push({path: '/create'})"
        />
    </div>

    <div class="flex row q-gutter-md">
    <div v-for="(document, index) in documents" :key="index" style="width: 300px;">
      <DocumentCard />
    </div>
</div>

  </q-page>
</template>

<script setup lang="ts">
import DocumentCard from 'src/components/DocumentCard.vue';
import { documents } from 'src/content/mock';

</script>
