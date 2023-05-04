<script setup>
import { ref } from 'vue'

const myValue = ref('')

function click() {
  fetch('https://tutbudeturl.com', {
    method: 'POST',
    body: JSON.stringify({
      phoneNumber: myValue.value
    })
  })
  .then(response => {
    console.log(response)
    // обработка ответа с сервера
  })
  .catch(error => {
    console.error(error)
    // обрабатывает ошибку
  })
}
</script>

<template>
  <div class="app">
    <form>
      <h1 class="multi">
        <span id="m">M</span>
        <span id="a">A</span>
        <span id="s">S</span>
      </h1>
      <p><b>Log in Sing up to access your account</b></p>
        <div class="input-container">
          <label for="phoneNumber">+7</label>
          <input id="phoneNumber" v-model="myValue" class="input"/>
          </div>
          <div class="btn">
            <button @click="click" class="cnt">Continue</button>
        </div>
    </form>
  </div>
</template>

<style scoped>
   
</style>
