<script>
export default{
  data: () => ({
    contador: 10,
  }),
  methods: {
    sumar() {
      this.contador++;
    },
    restar() {
      this.contador--;
    },
    reset() {
      this.contador = 10;
    }
  },
}
</script>

<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="logo" width="125" height="125">
    <small><h1>Hola Mundo desde vue.js 3</h1></small>
    <hr>
    <h2>Contador: {{ contador }}</h2>
    <button @click="sumar()">+1</button>
    <button @click="restar()">-1</button>
    <button @click="reset()">Reset</button>
  </div>
</template>
<style scoped>
.container{
 text-align: center;
}
small{
  color: #666;
}
h1 {
  font-weight: bolder;
}
h2 {
  font-size: 2.5rem;
}
button{
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0 0 1rem 1rem;
}
</style>

