<template>
  <q-page class="q-pa-lg">
    <q-btn
      icon="arrow_back_ios"
      label="Voltar"
      flat
      rounded
      @click="$router.back()"
      class="q-mb-lg"
    />

    <div class="flex row no-wrap q-mb-md" style="min-height: 150vh;">
      <div
        class="q-pa-md"
        style="
          width: 40%;
          max-width: 1000px;
          border-radius: 8px;
          position: sticky;
          top: 50px;
          align-self: start;
        "
      >
        <FormCreateDocument
          @title="setTitle()"
        />
      </div>

      <div
        style="
          width: 60%;
          margin-left: 10px;
          max-width: 1000px;
          border-radius: 8px;
          box-shadow: 2px 2px 2px 2px #ccc;
          padding: 10px;
        "
      >
        <NewDocument
          :title="title"
        />
      </div>
    </div>
  </q-page>
</template>

<script setup lang="ts">
import FormCreateDocument from 'src/components/FormCreateDocument.vue';
import NewDocument from 'src/components/NewDocument.vue';
import { ref } from 'vue';

const title = ref('');

function setTitle(value) {
  title.value = value;
}
</script>
