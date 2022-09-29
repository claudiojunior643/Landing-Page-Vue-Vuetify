<template>
  <main>
    <div class="main">
      <SectionMultiWord />
      <div class="CardsMain">
        <CardsMultiWord
          img="img1.jpeg"
          title="Conheça o Vuetify"
          text="Vuetify é um framework progressivo que tenta levar o
              desenvolvimento web para o próximo nível. Para melhor realizar
              esta tarefa, alguns sacrifícios tiveram que ser feitos em termos
              de suporte para versões antigas do Internet Explorer. Esta não é
              uma lista completa dos navegadores compatíveis, mas sim dos
              principais."
        />
        <CardsMultiWord
          img="img2.png"
          title="Conheça os três Pilares do Front-End"
          text="HTML é o componente básico da web, ele permite inserir o conteúdo
              e estabelecer a estrutura básica de um website. Portanto, ele
              serve para dar significado e organizar as informações de uma
              página na web. CSS é chamado de linguagem Cascading Style Sheet e
              é usado para estilizar elementos escritos em uma linguagem de
              marcação como HTML. O CSS separa o conteúdo da representação
              visual do site. JavaScript é uma linguagem de programação que
              permite a você implementar itens complexos em páginas web — toda
              vez que uma página da web faz mais do que simplesmente mostrar a
              você informação estática — mostrando conteúdo que se atualiza em
              um intervalo de tempo, mapas interativos ou gráficos 2D/3D
              animados, etc. — você pode apostar que o JavaScript provavelmente
              está envolvido."
        />
        <CardsMultiWord
          img="img3.png"
          title="Oque é Vue?"
          text="é um framework progressivo para a construção de interfaces de
              usuário. Ao contrário de outros frameworks monolíticos, Vue foi
              projetado desde sua concepção para ser adotável incrementalmente.
              A biblioteca principal é focada exclusivamente na camada visual
              (view layer), sendo fácil adotar e integrar com outras bibliotecas
              ou projetos existentes. Por outro lado, Vue também é perfeitamente
              capaz de dar poder a sofisticadas Single-Page Applications quando
              usado em conjunto com ferramentas modernas e bibliotecas de apoio."
        />
      </div>
    </div>
  </main>
</template>

<script>
import SectionMultiWord from "@/components/MainComponents/MainSection.vue";
import CardsMultiWord from "@/components/MainComponents/MainCards.vue";
export default {
  name: "MainMultiWord",
  components: {
    SectionMultiWord,
    CardsMultiWord,
  },
};
</script>
  
  <style lang="scss" scoped>
.main {
  background-color: #eb5f2e;
}
.CardsMain {
  display: flex;
  justify-content: space-around;
  padding-bottom: 100px;
}
@media (max-width: 700px) {
  .CardsMain {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
}
</style>