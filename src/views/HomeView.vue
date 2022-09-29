<template>
  <div class="home">
    <HeaderMultiWord />
    <MainMultiWord />
    <FooterMultiWord />
  </div>
</template>

<script>
// @ is an alias to /src
import HeaderMultiWord from "@/components/header.vue";
import MainMultiWord from "@/components/main.vue";
import FooterMultiWord from "@/components/footer.vue";

export default {
  name: "HomeView",
  components: {
    HeaderMultiWord,
    MainMultiWord,
    FooterMultiWord,
  },
};
</script>
