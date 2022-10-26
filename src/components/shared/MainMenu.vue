<script setup>
import menus from "@/data/menus.json";
import { RouterLink } from "vue-router";
import { library } from "@fortawesome/fontawesome-svg-core";
import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";
import { faChevronDown } from "@fortawesome/free-solid-svg-icons";
library.add(faChevronDown);
</script>
<template>
  <ul v-if="menus.main.length > 0" class="menu menu-horizontal p-0">
    <li
      v-for="menuItem in menus.main"
      :key="menuItem.id"
      :tabindex="menuItem.id"
    >
      <RouterLink :to="menuItem.url">
        {{ menuItem.name }}
        <font-awesome-icon
          v-if="menuItem.submenu.length > 0"
          icon="fa-solid fa-chevron-down"
        />
      </RouterLink>
      <ul
        v-if="menuItem.submenu.length > 0"
        class="p-2 shadow bg-base-100 rounded-box w-52 border-2 border-accent"
      >
        <li v-for="subMenuItem in menuItem.submenu" :key="subMenuItem.id">
          <RouterLink :to="subMenuItem.url">{{ subMenuItem.name }}</RouterLink>
        </li>
      </ul>
    </li>
  </ul>
</template>
