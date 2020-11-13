<template>
 <div>
  <v-col lg="6" md="6">
  <v-select class="menu"
    :items="['keeru', 'appu', 'rama', 'mounika']"
    label="Select Staff">
    <template v-slot:item="{ item, attrs, on }">
      <v-list-item
        v-bind="attrs" v-on="on">
        <v-list-item-title
          :id="attrs['aria-labelledby']"
          v-text=item>
		</v-list-item-title>
      </v-list-item>
     </template>
    </v-select>
  </v-col>
 </div>
</template>

<style scoped>
.menu{
  margin-top: 50px;
  padding-left: 1px;
  text-align: center;
}
</style>