

<template>
  <Navbar/>
  <div class="main-content">
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <Button/>
  <Card v-for="anime in animes" :anime="anime"> </Card>
  <Footer/>
</template>

<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'
import Button from './components/Button.vue'
import Card from './components/Card.vue'
import { ref } from "vue";

var animes = ref(
            [{title: 'Chainsawman',
            description: 'pretty messed up anime, dont watch if want mental health',
            content: 'devils, boobs and a silly main char'},
            {title: 'Bleach',
            description: 'hot redhair main character with a huge blade',
            content: 'maybe that didnt sound well'},
            {title: 'SpyxFamily',
            description: 'psychic kiddo, assasin wife and spy husband',
            content: 'happy family indeed'}
            ]
    ) 

</script>

<style scoped>
.main-content{
  display: flex;
    justify-content: center;
    align-items: center;
}
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
