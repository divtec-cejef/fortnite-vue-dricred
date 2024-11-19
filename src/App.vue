<template>
  <v-app>
    <AppHeader />
    <v-main>
      <router-view />
    </v-main>
    <AppFooter />
  </v-app>
</template>

<script setup>
  // Import du magasin des armes
    import {useArmeStore} from "@/stores/armeStore";
  // Charge le magasin des armes
  const armeStore = useArmeStore();
  // Affiche le nom des armes dans la console
  for( let arme of armeStore.armes){
    console.log(arme.nom);
  }
</script>

<style scoped>
body {
  background: url("/img/fortnite-convergence.jpg") no-repeat center center fixed;
  background-size: cover;
  font: 1rem "Lato", Arial, sans-serif;
  color: #101014;
  margin: 0;
  padding: 0;
}

img {
  max-width: 100%;
  height: auto;
  width: auto;
}
</style>
