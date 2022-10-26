<script setup>
import { computed } from "vue";
const appTitle = import.meta.env.VITE_APP_TITLE;
const fromDate = import.meta.env.VITE_APP_FROM_DATE;
const toDate = computed(() => {
  return new Date().getFullYear();
});
</script>

<template>&copy; {{ fromDate }}-{{ toDate }} {{ appTitle }}</template>
