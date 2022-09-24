<template>
  <div class="my-first-block">
    <h1>{{fructName}}</h1>
  </div>
</template>

<script setup>
import {defineProps, toRefs} from "vue"

const props = defineProps({
    fructName: String
});

const {fructName} = toRefs(props);
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .my-first-block{
        width: 300px;
        background-color: silver;
        margin-bottom: 5px;
    }
</style>
