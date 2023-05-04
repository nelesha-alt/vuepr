<script setup>

</script>

<template>
  <div class="app">
    <form>
      <h1 class="multi">
        <span id="m">M</span>
        <span id="a">A</span>
        <span id="s">S</span>
      </h1>
      <p>Log in Sing up to access your account</p>
        <div class="input-container">
          <label for="phoneNumber">+7</label>
          <input id="phoneNumber" v-model="myValue" class="input"/>
          <div class="btn">
            <button @click="click" class="cnt">Continue</button>
          </div>
        </div>
    </form>
  </div>
</template>

<style scoped>
   
</style>
