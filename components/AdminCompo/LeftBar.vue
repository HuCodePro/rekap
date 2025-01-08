<script setup>
import { ref } from 'vue';

// Variables pour gérer les menus déroulants
const isDashboardOpen = ref(false);
const isClientOpen = ref(false);
const isEnterpriseOpen = ref(false);

const toggleMenu = (menu) => {
  if (menu === 'dashboard') isDashboardOpen.value = !isDashboardOpen.value;
  if (menu === 'client') isClientOpen.value = !isClientOpen.value;
  if (menu === 'enterprise') isEnterpriseOpen.value = !isEnterpriseOpen.value;
};
</script>

<template>
  <!-- Barre Latérale Gauche -->
  <div id="leftBar" class="fixed left-0 top-0 h-full w-[280px] bg-white border-r-2 border-purple-200 shadow-md flex flex-col p-5 space-y-6">
    
    <!-- Logo Section -->
    <div id="logoAdmin" class="flex items-center gap-4">
      <img class="w-20 h-20 rounded-full shadow-md" src="/adminLogo.png" alt="photo admin" />
      <p class="uppercase text-2xl font-bold text-purple-600">Rekadmin</p>
    </div>

    <!-- Section Menu Principal -->
    <ul class="space-y-4 mt-6">

      <!-- Dashboard Menu -->
      <li @click="toggleMenu('dashboard')" class="menu-item mt-10">
        <div class="flex justify-between items-center">
          <p class="uppercase font-medium text-purple-600">Dashboard</p>
          <span :class="{'rotate-180': isDashboardOpen}" class="transition-transform duration-300">▼</span>
        </div>
        <ul v-if="isDashboardOpen" class="submenu">
          <li class="submenu-item">Sales</li>
          <li class="submenu-item">Projects</li>
          <li class="submenu-item">Statistics</li>
        </ul>
      </li>
      <!-- Clients -->
      <li @click="toggleMenu('client')" class="menu-item">
        <div class="flex justify-between items-center">
          <p class="uppercase font-medium text-purple-600">Clients</p>
          <span :class="{'rotate-180': isClientOpen}" class="transition-transform duration-300">▼</span>
        </div>
        <ul v-if="isClientOpen" class="submenu">
          <li class="submenu-item">Création de Compte</li>
          <li class="submenu-item">Ajout de Collaborateurs</li>
        </ul>
      </li>

      <!-- Entreprise -->
      <li @click="toggleMenu('enterprise')" class="menu-item">
        <div class="flex justify-between items-center">
          <p class="uppercase font-medium text-purple-600">Entreprise</p>
          <span :class="{'rotate-180': isEnterpriseOpen}" class="transition-transform duration-300">▼</span>
        </div>
        <ul v-if="isEnterpriseOpen" class="submenu">
          <li class="submenu-item">Création de Compte</li>
          <li class="submenu-item">Ajout de Collaborateurs</li>
        </ul>
      </li>


      <!-- Gestionnaire de Projet -->
      <li class="menu-item">Gestionnaire de Projet</li>

      <!-- Envoi de Factures et Devis -->
      <li class="menu-item">Envoi de Facture & Devis</li>

      <!-- Envoi de Compte Rendu -->
      <li class="menu-item">Envoi de Compte Rendu</li>

      <!-- Tickets Clients -->
      <li class="menu-item">Tickets Clients</li>

      
      <!-- Historique des Avancées -->
      <li class="menu-item">Historique des Avancées</li>

      <!-- Abonnement -->
      <li class="menu-item">Abonnement</li>

    </ul>
  </div>
</template>

<style scoped>
#leftBar {
  z-index: 50;
  overflow-y: auto;
}

/* Style Général des Éléments du Menu */
.menu-item {
  @apply w-full text-left px-4 rounded-lg border border-purple-300 bg-purple-50 hover:bg-purple-100 transition-all duration-300 shadow-sm cursor-pointer py-2;
}

/* Sous-menus */
.submenu {
  @apply mt-2 space-y-2 pl-4;
}

.submenu-item {
  @apply h-[50px] text-left rounded-lg border border-purple-200 bg-purple-50 hover:bg-purple-100 transition-all duration-300 flex items-center px-4 cursor-pointer;
}

/* Rotation de l'icône ▼ */
.rotate-180 {
  transform: rotate(180deg);
}
</style>
