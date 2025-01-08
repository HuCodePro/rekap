<script>
export default {
  data() {
    return {
      form: {
        name: "",
        email: "",
        message: "",
      },
      successMessage: "",
    };
  },
  methods: {
    handleSubmit() {
      this.successMessage = "Votre message a été envoyé avec succès ! Merci.";
      this.form.name = "";
      this.form.email = "";
      this.form.message = "";
    },
  },
};
</script>

<template>
  <div class="max-w-xl mx-auto p-6 bg-white shadow-xl shadow-gray-300 rounded-lg">
    <h2 class="text-2xl font-bold mb-6 text-gray-800">Contactez-nous</h2>
    <form @submit.prevent="handleSubmit">
      <div class="mb-4">
        <label for="name" class="block text-gray-700 font-semibold mb-2">Nom</label>
        <input
            v-model="form.name"
            type="text"
            id="name"
            placeholder="Votre nom"
            class="w-full p-3 border bg-white rounded-lg focus:outline-none focus:ring-2 focus:ring-[#52489C]"
            required
        />
      </div>
      <div class="mb-4">
        <label for="email" class="block text-gray-700 font-semibold mb-2">Email</label>
        <input
            v-model="form.email"
            type="email"
            id="email"
            placeholder="Votre email"
            class="w-full p-3 border bg-white rounded-lg focus:outline-none focus:ring-2 focus:ring-[#52489C]"
            required
        />
      </div>
      <div class="mb-4">
        <label for="message" class="block text-gray-700 font-semibold mb-2">Message</label>
        <textarea
            v-model="form.message"
            id="message"
            rows="5"
            placeholder="Votre message"
            class="w-full p-3 border bg-white rounded-lg focus:outline-none focus:ring-2 focus:ring-[#52489C]"
            required
        ></textarea>
      </div>
      <button
          type="submit"
          class="w-full bg-[#52489C] text-white font-bold py-3 rounded-lg hover:bg-[#3E377E] transition-colors"
      >
        Envoyer
      </button>
    </form>
    <p v-if="successMessage" class="mt-4 text-green-600 font-bold">{{ successMessage }}</p>
  </div>
</template>