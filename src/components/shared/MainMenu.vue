<script setup>
import menus from "@/data/menus.json";
import MenuItem from "@/components/menu/MenuItem.vue";
const menu = menus.main;
</script>
<template>
  <ul
    v-if="menu.length > 0"
    class="menu menu-horizontal p-0 rounded-lg bg-inherit text-inherit"
  >
    <MenuItem
      v-for="(item, index) in menu"
      :key="index"
      v-bind="{ name: item.name, path: item.path, submenu: item.submenu }"
    ></MenuItem>
  </ul>
</template>
