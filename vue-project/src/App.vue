<script setup>
import Deskarado from './components/Deskarado.vue';
import Debichos from './components/Debichos.vue';
import Acontraluz from './components/Acontraluz.vue';
import Destilar from './components/Destilar.vue';
import Rating from './components/Rating.vue';







</script>

<template>

    
 <div class="prueba">
  <div class="Cards">
    
    <div class="sombra">
      <div class="conrating">
        <Deskarado/>
        <Rating :max-rating="5" :initial-rating="3" @rating-selected="handleRatingSelected" />
    
      </div>

    </div>
    
    
    
    <div class="sombra">
      <div class="conrating">
      <Debichos/>
      <Rating :max-rating="5" :initial-rating="3" @rating-selected="handleRatingSelected" />
    
    
      </div>
    </div>
    
    
    
    <div class="sombra">
      <div class="conrating">
      <Acontraluz/>
      <Rating :max-rating="5" :initial-rating="3" @rating-selected="handleRatingSelected" />
      </div>
    </div>
    

    <div class="sombra">
      <div class="conrating">
      <Destilar/>
      <Rating :max-rating="5" :initial-rating="3" @rating-selected="handleRatingSelected" />
    </div>
    </div>
    

</div>

</div> 



 
</template>

<style scoped>

.prueba {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  align-content: center;
  
}
.conrating {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.Cards {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 25px;
  max-width: 100%;
}

.sombra {
  border: solid 0.1px rgb(61, 59, 59);
  margin: 10px;
  height: auto;
}
.sombra:hover {
  cursor: pointer;
  box-shadow: inset 1px 2px 20px 0 blue;
}





</style>
