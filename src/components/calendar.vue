<template>
  <div class="calendar">
  <v-row >
    <v-date-picker  v-model="picker" header-color="blue"></v-date-picker>
     </v-row>
  <h4>{{picker}}</h4><br>
  <h3>Add Your Details</h3><br>
  <input type="text" placeholder="abc"  style="align-center" /><br><br>
     <input type="tel" placeholder="+91|mobile number"/><br>
     <br>
     <input type="mail" placeholder="Example@gmail.com"/><br><br>
       <input type="text" placeholder="Address(optional)"/><br><br>
      
  </div>
  
</template>

<script>
  export default {
    data () {
      return {
        picker: new Date().toISOString().substr(0, 10),
        
      }
    },
  }
</script>

<style>
   .calendar{
     padding-left: 200px;
     
        }
</style>
  

