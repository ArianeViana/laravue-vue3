<template>
  <div id="componentes">
    <h1>Teste de Componentes</h1>
  </div>
</template>

<script>
export default {
  name: "TheHeader",
};
</script>

<style scoped>
#componentes {
  display: flex;
  justify-content: center;
}

h1 {
  background-color: black;
  color: white;
  width: 300px;
  text-align: center;
}
</style>
