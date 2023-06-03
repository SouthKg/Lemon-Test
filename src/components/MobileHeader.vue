<template>
  <div class="row">
    <div class="column logo">
      <img class="logo" src="../assets/logo-veolia.png" href="/">
    </div>
    <div class="column burger">
      <button @click="toggleDropdown"></button>
        <div v-if="showDropdown">
          <ul>
            <li>Option 1</li>
            <li>Option 2</li>
            <li>Option 3</li>
          </ul>
        </div>
    </div>
  </div>
  <div class="row">
    <div class="search-bar">
      <input type="text" placeholder="Recherche"><button type="submit"></button>
    </div>
  </div>

</template>


<script>
export default {
  name: "MobileHeader",

  data() {
    return {
      showDropdown: false
    };
  },
  methods: {
    toggleDropdown() {
      this.showDropdown = !this.showDropdown;
    }
  }
};
</script>

<style>
button {
  display: inline-block;
  background-color: transparent;
  border: none;
  cursor: pointer;
  background-image: url("../assets/menu.png");
  background-repeat: no-repeat;
  background-position: center center;
  background-color:white;
  border: solid 1px #6C757D;
  height:40px;
  width:80px;
}

ul {
  list-style: none;
  padding: 0;
  margin: 0;

}

li {
  padding: 8px;
  background-color: #f1f1f1;
  border-bottom: 1px solid #ccc;
}

.dropdown {
  display: none;
}

.show {
  display: block;
}
.dropdown {
  display: none;
  transition: all 0.3s ease;
}

.show {
  display: block;
}

.row{
  display:flex;
  flex-direction: row;
}

.column{
  display:flex;
}
.column.logo{
  width:70%
}
.column.burger{
  width:30%;
  justify-content: end;
}

.search-bar{
  display: flex;
}

.search-bar input[type=text] {
  float: right;
  border: none;
  font-size: 17px;
  height:36px;
  border:solid 1px #6C757D;
  width:280px;
  padding-left:15px;
}
.search-bar button{
  background:#6C757D;
  height:40px;
  width:40px;
  background-image: url("../assets/Search.png");
  background-position:center center;
  background-repeat: no-repeat;
  border:solid 1px #6C757D;
  cursor: pointer;
}

</style>
