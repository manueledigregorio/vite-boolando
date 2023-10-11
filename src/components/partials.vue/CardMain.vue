<script>
export default {
  name: 'CardMain',

  props: {
    card:Object,
  },
}
</script>

<template>
  
  <div class="product">
    <div class="switch">
      <img  class="modello uno" :src="`../../src/assets/img/${card.primaryImage}`" alt="">
      <img  class="modello due" :src="`../../src/assets/img/${card.secondaryImage}`" alt="">
    </div>
    <div class="lable">
      <span v-if="card.discount !== null" class="discount">{{ card.discount }}</span>
      <span v-if="card.sostenibilita === true" class="green">Sostenibilità</span>
    </div>
    <span class="hearts">&hearts;</span>
    <span>{{ card.marca }}</span>
    <h2>{{ card.modello }}</h2>
    <span class="euro-red">{{ card.lastPrice }} &euro;</span> <span class="euro-bar">{{ card.fullPrice }} </span>
  </div>

</template>


<style lang="scss" scoped>
  @use '../../scss/partials/General.scss' as *;
  @use '../../scss/partials/typography.scss' as *;
  @use '../../scss/partials/variabiles.scss' as *;

  .product{
    position: relative;
    width:calc(100% / 3.1);
    margin-bottom: 50px;


    .modello{
        width: 100%;
        height: auto;
        cursor: pointer;
    }

    .switch:hover .modello.uno{
        display: none;

    }

    .switch:hover .modello.due{
        display: block;
    }

    .modello.uno {
          display: block;
    }
    .modello.due{
        display:none ;
    }

    .lable{
        position: absolute;
        bottom: 120px;
        left:0px;
        color: white;
        font-size: 0,8rem;

        .discount{
            background-color: red;
            padding: 3px 3px;
        }
        .green{
            background-color: green;
            padding: 3px 5px;
        }

        
    }

    .hearts{
        position: absolute;
        top:10px;
        right: 0px;
        padding: 5px 5px;
        background-color: white;

    }

    .euro-red{
        color: red;
    }

    .euro-bar{
        text-decoration: line-through;
    }
  }
    

</style>