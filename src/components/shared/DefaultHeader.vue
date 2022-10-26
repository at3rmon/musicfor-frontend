<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
  <header>
    <div>
      <nav>
        <ul>
          <li><RouterLink to="/">Home</RouterLink></li>
          <li><RouterLink to="/about">About</RouterLink></li>
        </ul>
      </nav>
    </div>

    <img alt="Vue logo" class="logo h-12" src="@/assets/logo.svg" />
  </header>
</template>
