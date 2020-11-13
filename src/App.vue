<template>
 <div id="app">
  <v-app>
    <v-main >
      <v-card>
        <v-col >
          <h2 style="text-align:center">calendar</h2>
          <v-row>
            <calendar/>
            <v-col>
              <Menu/>
              <appointment/>
            </v-col>
          </v-row>
        </v-col>
        <v-col >
          <h4 style="text-align:center">Add your details</h4>
          <v-row>
            <detail/>
            <feedback/>
          </v-row>
        </v-col>
        <v-col>
          <v-flex>
          <v-btn class="btn" rounded elevation="30" color="primary" 
          style="width:150px">Book</v-btn>
          </v-flex>
        </v-col>
      </v-card>
      </v-main>
   </v-app>
 </div>
</template>

<script>
import detail from './components/detail';
import calendar from './components/calendar';
import Menu from './components/Menu';
//import store from './store';
import appointment from './components/appointment';
import feedback from './components/feedback';


export default {
  name: 'App',

  components: {
    calendar,
    Menu,
    appointment,
    feedback,
    detail,
  },
};
</script>

<style scoped>
.layout{
  width:1010px;
  height: 1200px;
}
.cal{
  margin-bottom: 50px;
  margin-top: 20px;
  margin-left: 500px;
  
}
.m1{
  margin-top: 50px;
}
.btn{
  margin-left: 600px;
}
</style>
