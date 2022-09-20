<template>
  <div id="condicionais">
    <h1>
      Teste de Condicionais
    </h1>

    <div v-show="showDiv">
      <p>V-show = true</p>
    </div>

    <div v-if="showNome">
      <p>V-if: {{ nome }}</p>
    </div>

    <div v-if="nivelAcesso == 'admin'">v-if / v-else-if / v-else: Usuário Admin</div>
    <div v-else-if="nivelAcesso == 'marketing'">v-if / v-else-if / v-else: Departamento Marketing</div>
    <div v-else="nivelAcesso == 'user'">v-if / v-else-if / v-else: User</div>

  </div>

  <!-- diferença entre v-show e v-if
          v-show: o elemento existe no DOM e usa um display:none para não ser exibido
          v-if: o elemento não existe no DOM quando é false-->

</template>

<script>
export default {
  name: "AsDiretivas",
  data() {
    return {
      showDiv: true,
      showNome: true,
      nome: "Ariane Viana",
      nivelAcesso: "marketing"
    }
  }
};
</script>

<style scoped>
#condicionais {
  background-color: burlywood;
  padding: 1px 10px 10px 10px;
  margin-bottom: 20px;
}
</style>
