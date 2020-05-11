<template>
  <div id="app" class="container">
    <header></header>
    <div class="sheet">      
      <Sheet/>
    </div>
    <footer></footer>   
  </div>
</template>

<script>
import Sheet from './components/sheet/Sheet.vue'

export default {
  name: 'App',
  components: {
    Sheet
  }
}
</script>

<style>
header {
  grid-area: header;
  background-color: #0E121D;
}
.sheet {
  grid-area: sheet;
  justify-self: center;
  padding-top: 50px;
  padding-bottom: 50px;
}

footer{
  grid-area: footer; 
  background-color: black;
}
.container{
  display: grid;
  grid-template-areas: 
  "header header header header"
  ". sheet sheet ."
  "footer footer footer footer";
  background-color:#E5E4EA;
}
</style>
