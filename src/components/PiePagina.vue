<template>
  <div>
    <h3>Sitio Web de Sonia Gutiérrez</h3>
    <h4>{{ mensaje }} - {{ telUser }}</h4>
    <h5>{{ dir }}</h5>
  </div>
</template>

<script>
export default {
  name: "piePagina",
  props: ["telUser", "dir"],
  data() {
    return {
      mensaje: "Librería especializada",
    };
  },
};
</script>

<style scoped>
div {
  background-color: aquamarine;
  width: 100%;
}
</style>