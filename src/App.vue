<template>
  <div id="app">
    <h1>Flashcard App!</h1>
    <FlashCardForm />
    <FlashCardList />
  </div>
</template>

<script>
import FlashCardForm from './components/FlashCardForm.vue'
import FlashCardList from './components/FlashCardList.vue'

export default {
  name: 'app',
  components: {
    FlashCardForm,
    FlashCardList
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
