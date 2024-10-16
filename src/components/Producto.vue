<!-- 2.- Pasar Props con Números
Crea un componente Producto que reciba el nombre y precio de un producto como props y muestre la información en un formato legible. -->

<template>
    <div class="card articulo">
      <div class="card-body">
        <h1>{{ nombre }}</h1>
        <p>{{ precio }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "Producto",
    props: ["nombre", "precio"],
  };
  </script>
  
  <style></style>