<script setup>
import MainMenu from "./MainMenu.vue";
import MainMobileMenu from "./MainMobileMenu.vue";
</script>

<template>
  <header class="sticky top-0 border-b-2 border-accent">
    <div class="navbar bg-base-100">
      <div class="navbar-start">
        <MainMobileMenu></MainMobileMenu>
        <RouterLink to="/"
          ><img alt="Vue logo" class="logo h-8" src="@/assets/logo.svg" />
        </RouterLink>
      </div>
      <div class="navbar-center hidden lg:flex">
        <MainMenu></MainMenu>
      </div>
      <div class="navbar-end">
        <div class="dropdown dropdown-end">
          <label tabindex="0" class="btn btn-ghost btn-circle avatar">
            <div class="w-10 rounded-full">
              <img src="https://placeimg.com/80/80/people" />
            </div>
          </label>
          <ul
            tabindex="0"
            class="mt-3 p-2 shadow menu menu-compact dropdown-content bg-base-100 rounded-box w-52"
          >
            <li>
              <a class="justify-between">
                Profile
                <span class="badge">New</span>
              </a>
            </li>
            <li><a>Settings</a></li>
            <li><a>Logout</a></li>
          </ul>
        </div>
      </div>
    </div>
  </header>
</template>
