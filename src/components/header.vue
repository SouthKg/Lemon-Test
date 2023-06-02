<template>
  <header>
    <img class="logo" src="../assets/logo-veolia.png" href="/">
    <div class="search-bar">
      <input type="text" placeholder="Recherche"><button type="submit"></button>
    </div>

    <nav>
      <ul>
        <li
            class="home"><a href="#" class="home"><img src="../assets/House.png"
                                                    alt="Accueil">
          Accueil
        </a></li>
        <li><a href="#"><img src="../assets/BoxSeam.png" alt="Produits"> Produits</a></li>
        <li><a href="#"><img src="../assets/Receipt.png" alt="Documentation">
          Documentation
        </a></li>
        <li><a href="#"><img src="../assets/PersonCircle.png" alt="Compte"> Compte</a></li>
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
  padding: 1% 17%;

  display: flex;
  align-items: center;
  justify-content: space-between;
}

nav ul {
  list-style-type: none;
  display: flex;

  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 16px;
  line-height: 24px;
}

nav ul li {
  margin-right: 10px;
}

nav ul li a {
  text-decoration: none;
  color: #6C757D;
  margin-right: 20px;
}
input[type=text] {
  float: right;
  border: none;
  font-size: 17px;
  height:36px;
  border:solid 1px #6C757D;
  width:280px;
  padding-left:15px;
}
button{
  background:#6C757D;
  height:40px;
  width:40px;
  background-image: url("../assets/Search.png");
  background-position:center center;
  background-repeat: no-repeat;
  border:solid 1px #6C757D;
  cursor: pointer;
}
.home{
  color:#F01018;
}
.logo{
  cursor: pointer;
}

.search-bar{
  display: flex;
}
ul img{
  margin-right:5px;
}
</style>