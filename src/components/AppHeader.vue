<script setup>

</script>

<template>
  <header>
  <nav>
    <ul class="navigation">
      <li><router-link to="/">Accueil</router-link></li>
      <li><router-link to="/nouvelle-carte">Présentation de Fortnite</router-link></li>
      <li><router-link to="/présentation">Nouvelle Carte</router-link></li>
    </ul>
  </nav>
  </header>
</template>

<style scoped>
header h1 {
  font-size: 3rem;
  color: white;
  text-align: center;
}

header .navigation {
  list-style-type: none;
  padding: 20px;
  display: flex;
  justify-content: center;
  background-color: rgba(0, 0, 0, 0.7); /* Fond noir semi-transparent */
  margin: 0;
}

header .navigation li {
  margin: 0 15px;
}

header .navigation a {
  color: white;
  text-decoration: none;
  font-weight: bold;
  padding: 10px 15px;
  transition: background-color 0.3s ease;
}

header .navigation li.actif a,
header .navigation a:hover {
  background-color: #FFFD03;
  color: #101014;
  border-radius: 5px;
}
</style>
