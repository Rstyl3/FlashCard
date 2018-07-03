<template>
    <div class="flashcard-form">
      <label for="front">Front
        <input v-model="newFront" type="text" id="front">
      </label>
      <label for="back">Back
        <input v-model="newBack" type="text" id="back">
      </label>
      <button>Add a New Card</button>
      <span class="error">Oops! Flashcards need a front and a back.</span>
    </div>
</template>

<script>
export default {
  name: 'FlashCardForm',
  props: {
  },
  data(){
    return{
      newFront: "",
      newBack:""
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.flashcard-form{
  position: relative;
}

label{
  font-weight: 400;
  color: #333;
  margin-right: 10px;
}

input{
  border-radius: 5px;
  border: 2px solid #eaeaea;
  padding: 10px;
  outline: none;
}

button{
  border-radius: 5px;
  border: 1px solid #87cb84;
  background-color: #87cb84;
  padding: 8px 15px;
  outline: none;
  font-size: 14px;
  font-weight: 700;
  color: #fff;
  cursor: pointer;
  transition: all 0.3s ease;
}

button:hover{
  background-color: #70a66f;
}

.error{
  margin-top: 10px;
  display: block;
  color: #e44e42;
  font-weight: 600;
}
</style>
