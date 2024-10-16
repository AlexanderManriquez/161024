<script>
import Tarjeta from "./components/Tarjeta.vue";

export default {
  components: {
    Tarjeta,
  },
  data() {
    return {
      articulos: [
        {
          nombre: "Martillo",
          descripcion:
            "Herramienta de percusión compuesta de una cabeza, por lo común de hierro, y un mango, generalmente de madera.",
        },
        {
          nombre: "Destornillador",
          descripcion:
            "Un destornillador es una herramienta que se utiliza para apretar y aflojar tornillos y otros elementos de máquinas que requieren poca fuerza de apriete.",
        },
      ],
    };
  },
};
</script>

<template>
  <div>
    <div v-for="articulo in articulos" :key="articulo">
      <Tarjeta :nombre="articulo.nombre" :descripcion="articulo.descripcion" />
    </div>
  </div>
</template>

<style scoped>
/* .logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
} */
</style>
