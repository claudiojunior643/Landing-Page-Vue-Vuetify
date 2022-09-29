<template>
  <header>
    <div class="header">
      <LogoMultiWord />
      <MenuMultiWord />
    </div>
  </header>
</template>

<script>
import LogoMultiWord from "@/components/HeaderComponents/LogoHeader.vue";
import MenuMultiWord from "@/components/HeaderComponents/MenuHeader.vue";
export default {
  name: "HeaderMultiWord",
  components: {
    LogoMultiWord,
    MenuMultiWord,
  },
};
</script>

<style lang="scss" scoped>
.header {
  background-color: #6108ff;
  height: 80px;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

@media (max-width: 900px) {
  .header {
    height: auto;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
}
</style>