<template>
<div id="main">
  <nav v-bind:class="active" v-on:click.prevent>
    <a href="#" class="home" v-on:click="makeActive('Accueil')">Accueil</a>
    <a href="#" class="projects" v-on:click="makeActive('Apropos')">À propos</a>
    <a href="#" class="services" v-on:click="makeActive('MentionsLegales')">Mentions Légales</a>
  </nav>
</template>

<style coped>
#nav {
  padding: 30px;
}
#nav a {
  font-weight: bold;
  color: #2c3e50;
}
#nav a.router-link-exact-active {
  color: white;
}
</style>