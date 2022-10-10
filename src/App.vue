<template>
 <div>
  <h1>{{mensaje}}</h1>
  <h2 v-text="texto"></h2>
  <input type="text" v-model="inputText"> 
  <img :src="img" alt="">
 </div>
</template>
<script>

export default ({
 name: "App", //a cada elemento se le debe colocar el nombre

 data() {//función donde retorna variables
  return{
    mensaje: "Hola Vue",
    texto: "hola texto",
    inputText: "",//para capturar el valor de un input
    img: "https://picsum.photos/id/237/200/300" //vbind aributos dinamicos
  }
 }

})
</script>

<style>

</style>
