<template>
  <div>
    <div class="MenuHeader">
      <a href="https://vuejsbr-docs-next.netlify.app/">Vue /</a>
      <a href="https://vuetifyjs.com/en/"> Vuetify /</a>
      <a href="#footer"> Redes</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "MenuMultiWord",
};
</script>

<style lang="scss" scoped>
a {
  font-size: 20px;
  color: #eb5f2e;
  font-weight: 200;
  text-decoration: none;
}
a:hover {
  color: white;
}
@media (max-width: 900px) {
  .MenuHeader {
    margin-bottom: 20px;
  }
}
@media (max-width: 600px) {
  a {
    font-size: 18px;
  }
}
</style>