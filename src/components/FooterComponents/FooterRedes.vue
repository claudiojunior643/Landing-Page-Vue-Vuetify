<template>
  <div>
    <div class="redes">
      <v-card class="CardFooter mx-auto" max-width="344" outlined>
        <v-list-item three-line>
          <v-list-item-content>
            <div class="text-overline mb-4">
              {{ title }}
            </div>
            <v-list-item-subtitle id="visita"
              >Link: {{ Link }}</v-list-item-subtitle
            >
          </v-list-item-content>

          <v-list-item-avatar tile size="80" color="grey"
            ><img :src="require('@/assets/' + logo)" alt=""
          /></v-list-item-avatar>
        </v-list-item>

        <v-card-actions>
          <v-btn class="ButtonRedes" outlined rounded text :href="Link">
            Visitar
          </v-btn>
        </v-card-actions>
      </v-card>
    </div>
  </div>
</template>

<script>
export default {
  name: "RedesMultiWord",
  props: {
    logo: String,
    title: String,
    Link: String,
  },
};
</script>

<style lang="scss" scoped>
.redes {
  font-size: 25px;

  #visita {
    font-size: 15px;
    font-weight: 600;
  }
  .CardFooter {
    background-color: #eb5f2e;
  }
  .ButtonRedes {
    background-color: #6108ff;
    color: white;
  }
}
@media (max-width: 800px) {
  .CardFooter {
    width: 300px;
  }
}
</style>