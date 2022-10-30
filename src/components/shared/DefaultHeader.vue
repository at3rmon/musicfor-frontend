<script setup>
import MainMenu from "./MainMenu.vue";
import MainMobileMenu from "./MainMobileMenu.vue";
</script>

<template>
  <header class="sticky top-0 z-50">
    <nav class="navbar bg-neutral text-neutral-content py-0">
      <div class="navbar-start">
        <MainMobileMenu></MainMobileMenu>
        <RouterLink to="/"
          ><img alt="Vue logo" class="logo h-8" src="@/assets/logo.svg" />
        </RouterLink>
      </div>
      <div class="navbar-center hidden lg:flex bg-inherit text-inherit">
        <MainMenu></MainMenu>
      </div>
      <div class="navbar-end">
        <div class="dropdown dropdown-end">
          <label
            tabindex="0"
            class="btn btn-ghost btn-circle avatar placeholder"
          >
            <div
              class="bg-neutral-focus text-neutral-content rounded-full w-24"
            >
              <span class="text-xl">CB</span>
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
    </nav>
  </header>
</template>
