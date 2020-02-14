<template>
  <div id="app">
    <h1 class="center">Conversor de Moedas</h1>
    <div class="linha">
      <Conversor moeda-a="USD" moeda-b="BRL"/>
      <Conversor moeda-a="BRL" moeda-b="USD"/>
    </div>
    <h3 class="center">Dólar dos EUA/Real brasileiro</h3>
    <hr />
    <div class="linha">
      <Conversor moeda-a="CAD" moeda-b="BRL"/>
      <Conversor moeda-a="BRL" moeda-b="CAD"/>
    </div>
    <h3 class="center">Dólar canadense/Real brasileiro</h3>
    <hr />
    <div class="linha">
      <Conversor moeda-a="EUR" moeda-b="BRL"/>
      <Conversor moeda-a="BRL" moeda-b="EUR"/>
    </div>
    <h3 class="center"> Euro/Real brasileiro</h3>
    <hr />
    <div class="linha">
      <Conversor moeda-a="BTC" moeda-b="BRL"/>
      <Conversor moeda-a="BRL" moeda-b="BTC"/>
    </div>
    <h3 class="center"> Bitcoin/Real brasileiro</h3>
    <hr />
     <div class="linha">
      <Conversor moeda-a="RUB" moeda-b="BRL"/>
      <Conversor moeda-a="BRL" moeda-b="RUB"/>
    </div>
    <h3 class="center"> Rublo russo/Real brasileiro</h3>
    <hr />
  </div>
</template>

<script>
import Conversor from "./components/Conversor.vue"

export default {
  name: 'App',
  components: {
    Conversor
  }
}
</script>

<style>
body{
  background: linear-gradient(to right, rgb(83, 105, 118), rgb(41, 46, 73));
}
#app {
  background-color: aliceblue;
  margin: auto;
  max-width: 900px;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}

.linha {
  margin-top: 40px;
  display: flex;
  justify-content: space-around;
}

@media (max-width: 600px) {
  .linha {
  display: inline;
}
  #app{
  max-width: 400px;
}
}
.center {
  text-align: center;
}

hr { 
  display: block;
  margin-bottom: 80px;
  border-width: 4px;
} 

</style>
