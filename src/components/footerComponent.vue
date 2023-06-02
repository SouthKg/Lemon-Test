<template>
  <footer class="footer">
    <div class="wave-background"></div>
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
}

.footer-columns {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  background: #212529;
}

.footer-column {
  width: 20%;
  padding: 10px;
}

.footer-column h3 {
  font-size: 18px;
}

.footer-column p {
  font-size: 14px;
  line-height: 1.4;
}

.footer-extra {
  text-align: center;
  background: #212529;
}

.footer-extra p{
  margin:0;
}

.wave-background{
  height:150px;
  background-image: url("../assets/backgroundfooter2.png");
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
}
</style>