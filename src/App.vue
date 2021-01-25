<template>
  <div id="app">
    <PiePagina :tel-user="telefono" dir="C/SerogioPo 24" />
    <h1>{{ mensaje }}</h1>
    <hr />
    <span> Libros disponibles:</span>
    <pedropo :libros="libros"> </pedropo>
    <hr />
    <PiePagina :tel-user="telefono" dir="C/Pajascu 25" />
  </div>
</template>

<script>
  import PiePagina from "./components/PiePagina.vue";
  import pedropo from "./components/listalibros.vue";

  export default {
    name: "App",
    components: {
      PiePagina,
      pedropo
    },
    data() {
      return {
        mensaje: "Librería Mi Mundo de Papel",
        telefono: 923451111,
        libros: [
          { titulo: "La villa de las telas" },
          { titulo: "La isla de las tormentas" },
          { titulo: "Dime quien soy" },
        ],
      };
    },
    methods: {
      mostrarAlerta() {
        alert("Número de libros almacenados:" + this.libros.length);
      },
    },
  };
</script>

<style>
  h1, h2, h3, h4, h5 {
    text-align: center;
  }

  
</style>