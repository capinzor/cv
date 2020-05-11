<template>
  <div class="contact-name">
    <div class="name">{{ msg }}</div>
    <div class="contact">
      <div class="address">
        <i class="fas fa-map-marker-alt"></i> 
        <span>  {{`Calle 189 # 8 - 24 casa 55, Bogotá`}}</span>
      </div>
      <div class="phone">
        <i class="fas fa-phone-alt"></i>
        <span>  {{' '+'3208984695'}}</span>
      </div>
      <div class="mail">
        <i class="fas fa-envelope"></i>
        <span>  {{' capinzonr@unal.edu.co'}}</span>
      </div>      
    </div>    
  </div>
</template>

<script>


export default {
  name: 'ContactName',
  
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url('https://fonts.googleapis.com/css?family=Bebas+Neue');
.name {
  grid-area: name;
  position: relative;
  white-space: pre-wrap;
  break-inside: auto;
  text-transform: uppercase;
  font-family: Bebas Neue;
  font-size: 36px;
  line-height: 36px;
  letter-spacing: 1.8px;
  color: rgb(99, 100, 102);
  word-break: break-word !important;
  padding: 64px 32px 64px 50px;
}
.contact{
  grid-area: contact;
  line-height: 23px;
  font-size: 14px;
  color: rgb(118, 119, 122);
  padding: 64px 32px;
}
.contact-name{
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-areas: 
  "name contact";
  border-bottom: 1px solid rgb(187, 188, 190);
}
span{  
  padding: 5px;
}
</style>
