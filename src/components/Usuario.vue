<!-- 4.-  Pasar Objetos como Props
Crea un componente Usuario que reciba como prop un objeto con la información de un usuario (nombre, apellido, edad) 
y muéstrelo en un formato de tarjeta. -->
<template>
    <div class="card">
        <div class="card-body">
            <h2 class="card-title">{{ user.name }} {{ user.lastName }}</h2>
            <p class="card-text">Edad: {{ user.age }}</p>
        </div>
    </div>
</template>

<script>
export default {
  name: "Usuario",
  props: {
    user: {
      type: Object,
    },
  },
};
</script>

<style scoped></style>
