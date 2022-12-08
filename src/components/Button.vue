<template>
    <button @click="(hello = !hello)"
    class="
      px-6
      py-2
      font-semibold
      text-white
      bg-blue-500
      rounded-md
      hover:opacity-80
      focus:outline-none">
    STFU
  </button>
  <h2 class="m-12" v-if="hello"> Hello! How are u?</h2>
  <h2  class="m-12" v-else> Oh, rude</h2>
</template>

<script setup>
    import { ref } from "vue";
    
    let hello = ref(true);
    

</script>