<script setup>
const appTitle = import.meta.env.VITE_APP_TITLE;
const fromDate = parseInt(import.meta.env.VITE_APP_FROM_DATE);
const toDate = new Date().getFullYear();
</script>

<template>&copy; {{ fromDate }}-{{ toDate }} {{ appTitle }}</template>
