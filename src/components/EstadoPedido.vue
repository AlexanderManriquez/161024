<!-- 5.-  Renderizado Condicional con Props
Crea un componente EstadoPedido que reciba como prop el estado de un pedido (por ejemplo, "enviado", "pendiente", "cancelado")
 y muestre un mensaje diferente dependiendo del estado. -->

<template>
    <div class="fw-bold my-4 display-6">
        <p class="text-success" v-if="estado === 'enviado'">El pedido ha sido enviado</p>
        <p class="text-warning" v-else-if="estado === 'pendiente'">El pedido está pendiente</p>
        <p class="text-danger" v-else-if="estado === 'cancelado'">El pedido ha sido cancelado</p>
        <p class="text-info" v-else>Estado desconocido</p>
    </div>
</template>

<script>
export default {
  name: "EstadoPedido",
  props: {
    estado: {
      type: String,
    },
  },
};
</script>

<style scoped></style>