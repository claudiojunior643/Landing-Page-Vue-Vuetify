<template>
  <div>
    <div class="logo">
      <img src="@/assets/comparacao-vuejs-reactjs.png" alt="" />
      <h1>Vue + Vuetify</h1>
    </div>
  </div>
</template>

<script>
export default {
  name: "LogoMultiWord",
};
</script>

<style lang="scss" scoped>
.logo {
  display: flex;
  align-items: center;
  color: white;
  img {
    height: 50px;
    width: 50px;
    border-radius: 100%;
    margin-right: 20px;
  }
}
@media (max-width: 900px) {
  .logo {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin-bottom: 10px;
    margin-top: 20px;
  }
  img {
    height: 20px;
    width: 20px;
    margin-right: 0;
  }
  h1 {
    font-size: 20px;
    margin-left: -10px;
  }
}
@media (max-width: 600px) {
  img {
    height: 15px;
    width: 15px;
  }
  h1 {
    // font-size: 18px;
    margin-left: -15px;
  }
}
</style>