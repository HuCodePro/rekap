<template>
  <div class="navbar bg-white rounded-3xl shadow-xl shadow-gray-300 ">
    <div class="navbar-start">
      <div class="dropdown">
        <div tabindex="0" role="button" class="btn btn-ghost btn-circle ">
          <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-5 w-5 text-custom"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor">
            <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h7" />
          </svg>
        </div>
        <ul
            tabindex="0"
            class="menu menu-sm dropdown-content bg-base-100 rounded-box z-[1] mt-3 w-52 p-2 shadow ">

          <li><a href="/">Acceuil</a></li>
          <li><a href="/">Panel</a></li>
          <li><a href="/about">Qui somme nous ?</a></li>
          <li><a href="/contact">Contact</a></li>

        </ul>
      </div>
    </div>
    <div class="navbar-center">
      <a class=" text-xl text-custom font-extrabold">.REKAP</a>
    </div>
    <div class="navbar-end">
      <a href="/profil">
        <button class="btn btn-ghost btn-circle transition duration-300">
          <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-5 w-5 text-custom"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor">
            <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M12 12c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm0 2c-2.67 0-8 1.34-8 4v2h16v-2c0-2.66-5.33-4-8-4z" />
          </svg>
        </button>
      </a>
      <button class="btn btn-ghost btn-circle">
        <div class="indicator">
          <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-5 w-5 text-custom"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor">
            <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M15 17h5l-1.405-1.405A2.032 2.032 0 0118 14.158V11a6.002 6.002 0 00-4-5.659V5a2 2 0 10-4 0v.341C7.67 6.165 6 8.388 6 11v3.159c0 .538-.214 1.055-.595 1.436L4 17h5m6 0v1a3 3 0 11-6 0v-1m6 0H9" />
          </svg>
          <span class="badge badge-xs badge-primary"></span>
        </div>
      </button>
    </div>
  </div>
</template>

<style>
.text-custom {
  color: #52489C;
}

</style>
<script setup lang="ts">
</script>