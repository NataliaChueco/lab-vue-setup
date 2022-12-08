<template>
    <div id="card" class="flex flex-col">
      <h3 class="text-xl mt-5">{{anime.title}}
      </h3>
      <p class="text-sm">{{anime.description}}</p>
      <p class="mt-2"></p>
      {{anime.content}}
    </div>
  </template>
  
  <script setup>
    const props = defineProps(["anime"]);
  </script>