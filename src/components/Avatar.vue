<!-- 3.- Controlar el Tipo de Prop
Crea un componente Avatar que reciba como prop la URL de una imagen de perfil y el tamaño de la imagen (en píxeles). 
Asegúrate de que el tamaño sea de tipo Number. -->
<template>
    <div>
        <img :src="imgProfile" :style="{ width: `${size}px`}" />
    </div>
</template>

<script>
export default {
  name: "Avatar",
  props: {
    imgProfile: String,
    size: Number,
  },
};
</script>

<style scoped>
img {
  border-radius: 50%;
}
</style>
