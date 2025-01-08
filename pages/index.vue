<script setup>
import NavCompo from "~/components/nav/NavCompo.vue";
</script>

<template>
  <div class="min-h-screen bg-gray-100 ">
      <nav class="p-6"> <NavCompo /> </nav>


    <section id="hero-section">
      <CardsBrowser/>
    </section>

    <div class="p-8" ></div>

    <section class="flex justify-center">
      <NuxtImg
          src="/collaboration.png"
          alt="collaboration image"
          class="w-[40%] h-auto"
      />
    </section>

    <section>
      <h1>
        salem
      </h1>
    </section>
  </div>
</template>