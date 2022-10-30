<script setup>
import { library } from "@fortawesome/fontawesome-svg-core";
import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";
import { faChevronDown } from "@fortawesome/free-solid-svg-icons";
library.add(faChevronDown);
defineProps({
  name: {
    type: String,
    required: true,
  },
  path: {
    type: String,
    required: true,
  },
  submenu: {
    type: Array,
    default: () => [],
  },
});
</script>

<template>
  <li class="bg-inherit text-inherit p-2">
    <RouterLink :to="path" class="hover:bg-accent/25 transition">
      {{ name }}
      <FontAwesomeIcon
        v-if="submenu.length"
        icon="fa-solid fa-chevron-down"
      ></FontAwesomeIcon>
    </RouterLink>
    <ul v-if="submenu.length" class="menu bg-inherit text-neutral-content">
      <MenuItem
        v-for="(item, index) in submenu"
        :key="index"
        v-bind="{ name: item.name, path: item.path, submenu: item.submenu }"
      ></MenuItem>
    </ul>
  </li>
</template>
