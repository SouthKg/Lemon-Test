<template>
  <header>
    <div class="logo">Logo</div>
    <div class="search-bar">Recherche</div>
    <nav>
      <ul>
        <li><a href="#">Accueil</a></li>
        <li><a href="#">Produits</a></li>
        <li><a href="#">Documentation</a></li>
        <li><a href="#">Compte</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "headerComponent"
}
</script>

<style scoped>
header {
  background-color: #f2f2f2;
  padding: 20px;
  display: flex;
  align-items: center;
}

.logo {
  font-size: 24px;
  font-weight: bold;
}

.search-bar {
  margin: 0 20px;
}

nav ul {
  list-style-type: none;
  display: flex;
}

nav ul li {
  margin-right: 10px;
}

nav ul li a {
  text-decoration: none;
  color: #333;
}
</style>