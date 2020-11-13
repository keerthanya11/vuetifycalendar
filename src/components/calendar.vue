<template>
  <div class="calendar">
    <h5>{{date}}</h5>
     <v-row >
       <v-date-picker v-model="date" header-color="primary" color="primary" ></v-date-picker>
     </v-row>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        date: new Date().toISOString().substr(0, 10),           
       } 
    }
  }
</script>

<style scoped>
   .calendar{
     margin-top: 50px;
     padding-left: 200px;     
        }
</style>
  

