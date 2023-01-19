<template>

  <div id="example1">
    <h1>você clicou em mim {{ contador }} vezes</h1>
    <button @click="somar()">Adicionar + 1</button>
    <button @click="remover()">remover - 1</button>
    <button @click="limpar()">limpar tudo</button>
  </div>
</template>
 
<script>

export default {
  data: () => ({
    contador: 0,
  }),
  methods: {
    somar() {
      this.contador++;
    },
    remover() {
      this.contador--;
    },
    limpar() {
      this.contador = 0;
    },
  },
};

</script>

<style>

html{
  background-color: #292929;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #ffffff;
  text-align: center;
  margin-top: 60px;
}
button{
background-color: red;
border-radius: 30px;
padding: 20px;
color: aliceblue;
font-size: 30px;
margin: 20px;
}
</style>