<script setup>
import { ref } from 'vue'
import {sayHello} from "../api/hell";
const message = ref("时间刺客后台")

const he = () =>{
  sayHello().then(req=>{
    console.log(req)
  })
}


</script>

<template>
  <h1>{{ message }}</h1>
  <q-btn color="primary" label="Primary" />

</template>

<style scoped>
a {
  color: #42b983;
}
</style>
