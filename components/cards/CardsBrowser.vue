<script setup lang="ts">
</script>

<template>
  <section class="flex flex-col items-center justify-center text-center mt-12 py-16">
    <h1 class="text-5xl font-extrabold dark mb-12">
      Votre équipe va adorer utiliser <span class="text-custom">.REKAP</span>
    </h1>

    <div class="mockup-window bg-gray-100 border shadow-lg w-11/12 lg:w-3/4 mx-auto rounded-xl">
      <div class="bg-gray-50 px-10 py-16 grid grid-cols-1 md:grid-cols-3 gap-8">

        <div class="bg-white shadow-md shadow-purple-900 rounded-xl p-8 transition hover:scale-105 hover:shadow-lg hover:shadow-purple-950">
          <h2 class="text-3xl font-bold text-gray-800 mb-4">Projets</h2>
          <p class="text-gray-600">
            Gérez vos projets efficacement grâce à une vue d'ensemble claire.
          </p>
        </div>

        <div class="bg-white shadow-md shadow-purple-900 rounded-xl p-8 transition hover:scale-105 hover:shadow-lg hover:shadow-purple-950">
          <h2 class="text-3xl font-bold text-gray-800 mb-4">Tâches</h2>
          <p class="text-gray-600">
            Attribuez des tâches et suivez leur avancement en temps réel.
          </p>
        </div>

        <div class="bg-white shadow-md shadow-purple-900 rounded-xl p-8 transition hover:scale-105 hover:shadow-lg hover:shadow-purple-950">
          <h2 class="text-3xl font-bold text-gray-800 mb-4">Équipe</h2>
          <p class="text-gray-600">
            Collaborez avec votre équipe et communiquez facilement.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<style>
.text-custom {
  color: #52489C;
}
</style>