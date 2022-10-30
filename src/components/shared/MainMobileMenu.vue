<script setup>
import menus from "@/data/menus.json";
import MenuItem from "@/components/menu/MenuItem.vue";
import { library } from "@fortawesome/fontawesome-svg-core";
import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";
import { faBars } from "@fortawesome/free-solid-svg-icons";
library.add(faBars);
const menu = menus.main;
</script>
<template>
  <div class="dropdown">
    <label tabindex="0" class="btn btn-ghost lg:hidden">
      <font-awesome-icon icon="fa-solid fa-bars" />
    </label>

    <ul
      v-if="menu.length > 0"
      class="menu menu-compact dropdown-content mt-3 p-2 rounded-lg"
    >
      <MenuItem
        v-for="(item, index) in menu"
        :key="index"
        v-bind="{ name: item.name, path: item.path, submenu: item.submenu }"
      ></MenuItem>
    </ul>
  </div>
</template>
