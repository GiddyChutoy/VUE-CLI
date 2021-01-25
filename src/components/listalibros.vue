<template>
    <ol v-if="libros.length > 0">
      <li v-for="(libro, index) in libros" :key="index">
        {{ libro.titulo }}
      </li>
    </ol>
</template>
<script>
export default {
    name:"pedropo",
    props: ["libros"]
}
</script>