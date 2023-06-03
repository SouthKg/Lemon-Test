<template>
  <div>
    <button @click="toggleDropdown">Menu</button>
    <div v-if="showDropdown">
      <ul>
        <li>Option 1</li>
        <li>Option 2</li>
        <li>Option 3</li>
      </ul>
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
</style>
