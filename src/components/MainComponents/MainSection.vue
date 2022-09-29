<template>
  <div>
    <div class="Section">
      <v-card elevation="4" id="CardSection">
        <div class="PriSection">
          <h1>Vue + Vuetify</h1>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. <br />
            Perferendis tenetur ea necessitatibus. <br />
            Accusamus expedita nostrum cumque <br />
            iure facilis animi iste at exercitationem vel, <br />
            consequatur quia, dolore dolor natus quas dolorem?
          </p>
          <br />
        </div>
      </v-card>

      <div class="ImgSection">
        <img src="@/assets/6177d8f5714a9152b56f3a7a_Front-end.gif" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionMultiWord",
};
</script>

<style lang="scss" scoped>
#CardSection {
  background-color: #eb5f2e;
}
.Section {
  display: flex;
  align-items: center;
  justify-content: space-around;
}
.PriSection {
  // color: rgb(113, 4, 255);
  color: white;
  h1 {
    font-size: 50px;
    margin-bottom: 20px;
  }
  padding: 40px;
}
@media (max-width: 900px) {
  .PriSection {
    h1 {
      font-size: 25px;
      margin-bottom: 5px;
    }
    p {
      font-size: 15px;
    }
    padding: 15px;
    width: 300px;
    height: 200px;
  }
  img {
    width: 280px;
    height: 280px;
  }
}
@media (max-width: 600px) {
  .PriSection {
    h1 {
      font-size: 20px;
      margin-bottom: 5px;
      margin-top: 30px;
    }
    p {
      font-size: 10px;
    }
    padding: 10px;
    width: 230px;
    height: 200px;
  }
  img {
    width: 150px;
    height: 150px;
  }
  #CardSection {
    margin-bottom: 30px;
    margin-top: 30px;
  }
}
@media (max-width: 500px) {
  img {
    width: 130px;
    height: 130px;
  }
}
</style>