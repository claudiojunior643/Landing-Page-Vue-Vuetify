<template>
  <div class="cards">
    <div>
      <v-card class="mx-auto" max-width="344">
        <v-img :src="require('@/assets/' + img)" height="200px"></v-img>

        <v-card-title> {{ title }} </v-card-title>

        <v-card-actions>
          <v-btn color="orange lighten-2" text> Explore </v-btn>

          <v-spacer></v-spacer>

          <v-btn icon @click="show = !show">
            <v-icon>{{ show ? "mdi-chevron-up" : "mdi-chevron-down" }}</v-icon>
          </v-btn>
        </v-card-actions>

        <v-expand-transition>
          <div v-show="show">
            <v-divider></v-divider>

            <v-card-text>
              {{ text }}
            </v-card-text>
          </div>
        </v-expand-transition>
      </v-card>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardsMultiWord",
  data: () => ({
    show: false,
  }),
  props: {
    img: String,
    title: String,
    text: String,
  },
};
</script>

<style lang="scss" scoped>
@media (max-width: 1100px) {
  .v-sheet.v-card:not(.v-sheet--outlined) {
    width: 250px;
  }
}
@media (max-width: 900px) {
  .v-sheet.v-card:not(.v-sheet--outlined) {
    width: 200px;
    margin: -20px;
  }
}
@media (max-width: 700px) {
  .v-sheet.v-card:not(.v-sheet--outlined) {
    width: 300px;
  }
}
</style>
