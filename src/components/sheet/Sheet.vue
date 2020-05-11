<template>
  <div class="sheet">    
    <aside class="side-section"> 
      <AboutMe/>  
    </aside>
    <section class="main">
      <ContactName msg="camilo andrés pinzón ruiz"/>
      <!-- <img alt="Vue logo" src="./assets/logoUN.png"> -->
    </section>
  </div>
</template>

<script>
import ContactName from './ContactName.vue'
import AboutMe from './AboutMe.vue'

export default {
  name: 'Sheet',
  components: {
    ContactName,
    AboutMe
  } 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.main{
  grid-area: main;
  background-color: #ffffff;  
}
.side-section{
  grid-area: side-section;  
  background-color: #434244;  
}
.sheet{
  width: 1000px;
  min-height: 1312.52px;
  height: inherit;
  display: grid;
  grid-template-columns: 1fr 2fr;
  grid-template-areas:
  "side-section main";  
}
</style>