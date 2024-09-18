<template>
  <q-layout view="lHh Lpr lFf">
    <q-header style="background-color: white;">
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          icon="sort"
          aria-label="Menu"
          @click="toggleLeftDrawer"
          class="text-primary"
        />

        <q-toolbar-title>
        </q-toolbar-title>

        <q-avatar color="primary" text-color="white">J</q-avatar>
      </q-toolbar>
    </q-header>

    <q-drawer
      v-model="drawer"
      show-if-above
      style="background-color: #F0F4FC;"
      :mini="leftDrawerOpen"
      bordered
    >
      <q-list>
        <div class="text-center q-my-md">
          <q-img
            src="../assets/logo.svg"
            spinner-color="white"
            width="30%"
          />
        </div>

        <q-separator class="q-mb-md"/>

        <EssentialLink
          v-for="link in linksList"
          :key="link.title"
          v-bind="link"
        />
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script setup lang="ts">
import { ref } from 'vue';
import EssentialLink, { EssentialLinkProps } from 'components/EssentialLink.vue';

defineOptions({
  name: 'MainLayout',
});

const linksList: EssentialLinkProps[] = [
  {
    title: 'Meus documentos',
    caption: 'Visualize seus documentos',
    icon: 'folder',
    link: 'https://quasar.dev',
  },
  {
    title: 'Configurações',
    caption: '',
    icon: 'settings',
    link: 'https://github.com/quasarframework',
  },
];

const leftDrawerOpen = ref(false);
const drawer = ref(true);

function toggleLeftDrawer() {
  leftDrawerOpen.value = !leftDrawerOpen.value;
}
</script>
