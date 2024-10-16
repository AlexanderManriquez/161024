
<script>
import Tarjeta from "./components/Tarjeta.vue";
import Avatar from "./components/Avatar.vue";
import Producto from "./components/Producto.vue";

export default {
  components: {
    Tarjeta, Avatar, Producto
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
    
    <Avatar
      imgProfile="https://scontent.fscl17-1.fna.fbcdn.net/v/t39.30808-6/227408029_205778354892214_6013986529669216619_n.jpg?_nc_cat=104&ccb=1-7&_nc_sid=6ee11a&_nc_eui2=AeHXm87Zt91OcN90wKmlaNSyr968WOg0f7mv3rxY6DR_ucLHn392lppO8f9PghXyydKSi4UgLP3LFBDclqeqn_u_&_nc_ohc=35qEzpJP2_cQ7kNvgGIvpHz&_nc_zt=23&_nc_ht=scontent.fscl17-1.fna&_nc_gid=A3r8lW1ah-TNJ6SL0I0421B&oh=00_AYAJoCMDgLGvCQ_ht86FCki2o34ECJXvXS7gw4XajIlhsw&oe=6715FBAC"
      size=300
    />

    <Producto
      nombre="Pack de vasos"
      precio=5990
    />
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
