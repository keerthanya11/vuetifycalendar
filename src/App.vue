<template>
<div id="app">
<v-app>
    <v-main >
      <v-layout row wrap>
        <v-flex lg6>
      <h1 class="cal">Calendar</h1>
      <calendar/>  
        </v-flex>
        <v-flex lg6>
          <v-layout column wrap lg3>
          <Menu class="m1"/><br><br>
          <v-flex lg3 row >
          <appointment/>
          </v-flex>
          </v-layout>
        </v-flex> 
      </v-layout>
        
    </v-main>
</v-app>
</div>
</template>

<script>
import calendar from './components/calendar';
import Menu from './components/Menu';
import appointment from './components/appointment';

export default {
  name: 'App',

  components: {
    calendar,
    Menu,
    appointment,
  },
};
</script>

<style scoped>
.cal{
  margin-top: 20px;
  margin-left: 500px;
  color:blue;
}
.m1{
  margin-top: 50px;
}
</style>
