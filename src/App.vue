<template>
  <div id="app">
    <fw-preview ref="preview"></fw-preview>
    <fw-lista :elements="elements"></fw-lista>
  </div>
</template>

<script>
import Lista from './components/Lista';
import Preview from './components/Preview';
import elements from './assets/datos.json';

export default {
  name: 'app',
  components: {
    'fw-lista': Lista,
    'fw-preview': Preview,
  },
  data() {
    return {
      elements
    }
  },

}
</script>

<style lang="postcss">
   
  @import url('https://fonts.googleapis.com/css?family=Montserrat:400,700');

:root {
  height: 100vh;
  --bgcolor: #ddd;
  --textcolor: #fff;
  background: #222;
  
}

#app {
  margin-top: 4em;
  display: flex;
  justify-content: center;
  max-width: 900px;
  margin: 4em auto;
}
</style>
