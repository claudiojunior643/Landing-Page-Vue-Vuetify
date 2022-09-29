<template>
  <footer >
    <div id="footer">
      <h1>// Footer //</h1>
      <div class="MainFooter">
        <RedesMultiWord
          class="Redes"
          logo="GitHub.png"
          title="Git Hub"
          Link="https://github.com/claudiojunior643"
        />
        <RedesMultiWord
          class="Redes"
          logo="linkedin.png"
          title="Linkedin"
          Link="https://www.linkedin.com/in/cl%C3%A1udio-junior-452716221/"
        />
      </div>
    </div>
  </footer>
</template>

<script>
import RedesMultiWord from "@/components/FooterComponents/FooterRedes.vue";
export default {
  name: "FooterMultiWord",
  components: {
    RedesMultiWord,
  },
};
</script>

<style lang="scss" scoped>
#footer {
  background-color: #6108ff;
  color: orange;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  h1 {
    font-size: 30px;
    margin-top: 30px;
  }
}
.MainFooter {
  display: flex;
  flex-direction: row;
}
.Redes {
  margin-right: 20px;
  margin-top: 25px;
  margin-bottom: 50px;
}
@media (max-width: 600px) {
  .MainFooter {
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
}
</style>