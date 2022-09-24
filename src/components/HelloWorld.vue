<template>
  <div>hello world</div>
  <MyFirstComponent v-for="item of myArray" :key="item" :fructName="item"/>
  <button @click="click">Кликни на меня</button>
  <p>текст</p>
</template>

<script setup>
import MyFirstComponent from './MyFirstComponent.vue';

const myArray = ['Ананас', 'Банан', 'Яблоко'];

function click() {
  alert("hello world!");
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
