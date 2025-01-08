<script>

import {defineComponent} from "vue";
import NavCompo from "~/components/nav/NavCompo.vue";
import ContactCompo from "~/components/cards/form/ContactCompo.vue";

export default defineComponent({
  components: {ContactCompo, NavCompo}
})
</script>

<template>
  <div class=" bg-gray-100">
    <nav class="p-6"> <NavCompo /> </nav>


    <section>
     <ContactCompo/>
    </section>

  </div>
</template>