<template> 
  <div id="detail">
    <v-col cols="100" md="30" lg="30">
      <v-text-field outlined label="Name" type="text" />
      <v-text-field outlined label="Mobile No" type="tel"/>
      <v-text-field outlined label="Email" type="mail" />
      <v-text-field outlined type="text" label="Address"/>
    </v-col>
  </div>
</template>

<style scoped>
#detail{
  padding-left: 200px;
}
</style>