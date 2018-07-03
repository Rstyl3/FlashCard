<template>
  <div id="app">
    <h1>Flashcard App!</h1>
    <FlashCardForm :value="cards" @addCard="handleAddCard"/>
    <FlashCardList :value="cards" />
  </div>
</template>

<script>
import FlashCardForm from './components/FlashCardForm.vue'
import FlashCardList from './components/FlashCardList.vue'
import cards from "./data/app.js";

export default {
  name: 'app',
  components: {
    FlashCardForm,
    FlashCardList
  },
  data(){
    return{
      cards: cards
    }
  },
  methods:{
    handleAddCard(v){
      this.cards = v
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  max-width: 100%;
  padding: 2em;
}

</style>
