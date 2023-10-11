<script>

  import card from '../data/card';
  import CardMain from './partials.vue/CardMain.vue'

export default {
  name: "Main",
  components:{
    CardMain

  },

  data() {
    return {
      card
    }
  },
};
</script>

<template>
  <main>
    <div class="container-main container">
      <CardMain v-for="(item, index) in card" 
      :key="index" 
      :card ='item'/>

    </div>
  </main>
</template>


<style lang="scss" scoped>
  @use '../scss/partials/General.scss' as *;
  @use '../scss/partials/typography.scss' as *;
  @use '../scss/partials/variabiles.scss' as *;

 
    .container-main{
        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;
        margin-top: 100px;
        margin-bottom: 50px;

   
    }     
</style>