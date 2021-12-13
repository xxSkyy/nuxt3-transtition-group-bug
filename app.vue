<script lang="ts" setup>
const list = ["Welcome", "to", "nuxt3"]
</script>

<template>
  <div class="box">
    <div class="wrapper">
      <h1>List test</h1>
      <transition-group class="test" name="fade" tag="ul">
        <li v-for="i in list" :id="i">{{ i }}</li>
      </transition-group>
    </div>
  </div>
</template>

<style>
* {
  padding: 0;
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
}

body {
  background-color: rgb(27, 27, 27);
  color: white;
}
</style>

<style scoped>
.box {
  height: 100vh;
  width: 100vw;
  display: flex;
  justify-content: center;
  align-items: center;
}

.wrapper {
  background-color: rgb(36, 51, 99);
  border-radius: 2rem;
  padding: 2rem;
}

ul {
  list-style-type: none;
  background-color: turquoise;
}

li {
  text-align: center;
  margin: 1rem 0;
}

h1 {
  font-size: 30px;
  font-weight: bold;
}
</style>