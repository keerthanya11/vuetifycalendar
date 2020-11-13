<template>
  <div>
    <h4 class="slots">Available TimeSlots</h4>
    <v-container class="container" >
    <v-row>
      <v-col 
        v-for="slot in slots"
      :key="slot">
        <v-btn class="grey con1" v-if="slot.isReserved==true">
          {{slot.time}}
        </v-btn>
        <v-btn class="green con2" v-if="slot.isReserved!=true">
          {{slot.time}}
        </v-btn>
      </v-col>
    </v-row>
  </v-container>
  </div>
</template>

<script>
export default {
  data(){
    return{
       slots:[
            {isReserved:true,time:'10AM'},
            {isReserved:true,time:'10:30AM'},
            {isReserved:false,time:'11AM'},
            {isReserved:true,time:'11:30AM'},
            {isReserved:true,time:'12PM'},
            {isReserved:true,time:'12:30PM'},
            {isReserved:false,time:'1PM'},
            {isReserved:true,time:'1:30PM'},
            {isReserved:false,time:'2PM'},
         ]
       }   
    }
}
</script>

<style scoped>
.container{
  width: 550px;
  margin-left: 150px;
  
}
.slots{
   margin-left:150px;
}
      
.con1{
   color: aqua;
   background-color: lightslategray;
   width: 100px;
   text-align: center;
 }
.con2{
   color: aqua;
   background-color: green;
   width: 100px;
   text-align: center;
 }

</style>
