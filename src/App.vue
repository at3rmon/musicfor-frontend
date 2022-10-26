<script setup>
import { RouterView } from "vue-router";
import DefaultHeader from "@/components/shared/DefaultHeader.vue";
import DefaultFooter from "@/components/shared/DefaultFooter.vue";
</script>

<template>
  <DefaultHeader></DefaultHeader>
  <RouterView />
  <DefaultFooter></DefaultFooter>
</template>
