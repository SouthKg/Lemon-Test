<template>
  <footer class="footer">
    <div class="footer-columns">
      <div class="footer-column">
        <h3>Comite largitionum</h3>
        <p>Praefecto utcum ina Crebro acciverat Postquam abierat timor Vero sic intellego</p>
      </div>
      <div class="footer-column">
        <h3>Dotis nomine futura</h3>
        <p>Praefecto utcum ina Crebro acciverat Postquam abierat timor Vero sic intellego</p>
      </div>
      <div class="footer-column">
        <h3>Aleis certant turpi sono</h3>
        <p>Praefecto utcum ina Crebro acciverat Postquam abierat timor Vero sic intellego</p>
      </div>
      <div class="footer-column">
        <h3>Patres conscripti</h3>
        <p>Praefecto utcum ina Crebro acciverat Postquam abierat timor Vero sic intellego</p>
      </div>
    </div>
    <div class="footer-extra">
      <p>Veolia demo test site | Lemon Interactive © 2022</p>
    </div>
  </footer>
</template>

<script>
export default {
  name: "footerComponent"
}
</script>

<style scoped>
.footer {
  background-color: #f0f0f0;
  padding: 20px;
}

.footer-columns {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}

.footer-column {
  width: 20%;
  padding: 10px;
}

.footer-column h3 {
  font-size: 18px;
  margin-bottom: 10px;
}

.footer-column p {
  font-size: 14px;
  line-height: 1.4;
}

.footer-extra {
  margin-top: 20px;
  text-align: center;
}
</style>