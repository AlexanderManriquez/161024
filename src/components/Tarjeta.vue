<!-- 1.- Mostrar Información Básica con Props
Crea un componente Tarjeta que reciba como props el nombre y la descripción de un artículo, y muéstralos dentro de una tarjeta -->

<template>
  <div class="card articulo">
    <div class="card-body">
      <h5 class="card-title">{{ nombre }}</h5>
      <p class="card-text">
        {{ descripcion }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Tarjeta",
  props: ["nombre", "descripcion"],
};
</script>

<style></style>
