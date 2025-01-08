<script>
</script>

<template>
  <div class="max-w-4xl mx-auto bg-white shadow-md rounded-lg p-6">
    <h2 class="text-2xl font-bold text-gray-800 mb-6">Profil de l'utilisateur</h2>
    <div class="mb-6">
      <div class="flex items-center space-x-4">
        <div class="w-16 h-16 rounded-full bg-gray-200 flex items-center justify-center text-2xl font-bold text-gray-600">

        </div>
        <div>
          <h3 class="text-lg font-bold text-gray-800">Hugo</h3>
          <p class="text-gray-600">Email : nanani@gmail.com</p>
        </div>
      </div>
    </div>
    <div class="mb-6">
      <h3 class="text-xl font-bold text-gray-800 mb-4">Entreprises affectées</h3>
      <ul class="space-y-4">
        <li
            <!--  v-for="company in companies"
            :key="company.id"-->
            class="bg-gray-50 p-4 rounded-lg shadow-sm"
        >
          <div class="flex justify-between items-center">
            <div>
              <h4 class="text-lg font-bold text-gray-800">GYB</h4>
              <p class="text-gray-600">Collaborateurs : Antwon - Robin - Romain - Laurent </p>
            </div>
            <span
                class="bg-blue-500 text-white px-4 py-1 rounded-lg text-sm font-semibold"
            >
               tâches
            </span>
          </div>
        </li>
      </ul>
    </div>
    <div>
      <h3 class="text-xl font-bold text-gray-800 mb-4">Tâches dédiées</h3>
      <ul class="space-y-4">
        <li
           <!-- v-for="task in tasks"
            :key="task.id"-->
            class="bg-white border-l-4 border-blue-500 p-4 rounded-lg shadow-sm"
        >
          <h4 class="text-lg font-bold text-gray-800">Refont acceuil</h4>
          <p class="text-gray-600">tu dois refaire la refont de lacceuil </p>
          <p class="text-sm text-gray-500">Date limite : 9 août</p>
        </li>
      </ul>
    </div>
  </div>
</template>

