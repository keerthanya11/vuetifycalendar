<template>
    <div>     
     <v-container v-for="timeslot in timeslots"
      :key="timeslot" 
     >
      <div class="con1" v-if="timeslot.isReserved==true">{{timeslot.time}}</div>
      <div class="con2" v-if="timeslot.isReserved!=true">{{timeslot.time}}</div>
      </v-container>
    </div>
</template>

<script>
export default {
    data:()=>({
       timeslots:[
          {isReserved:true,time:'10AM'},
          {isReserved:true,time:'10:30AM'},
          {isReserved:false,time:'11AM'},
          {isReserved:true,time:'11:30AM'},
          {isReserved:true,time:'12PM'},
          {isReserved:true,time:'12:30PM'},
          {isReserved:false,time:'1PM'},
          {isReserved:true,time:'1:30PM'},

       ],
    })
}
</script>

<style scoped>
  .con1{
    background-color: grey;
   }
  .con2{
      background-color: green;
   }
</style>