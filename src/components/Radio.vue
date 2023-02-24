<template>
  <div
    v-on:click="activarRadio"
    class="flex border-black bg-white justify-center rounded-md overflow-hidden cursor-pointer">
    <div :class="fondoOp1">
        <p>3.3</p>
    </div>
    <input
    class="hidden"
      type="radio"
      :checked="checked"
    />
    <div :class="fondoOp2">
        <p>4.0</p>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
let checked = ref(true);
function activarRadio() {
    if (checked.value) {
        cambiarColor()
        checked.value = false;
    } else {
        cambiarColor()
        checked.value = true;
    }
    console.log(checked.value)
}

let fondoOp1 = ref("text-center bg-blue-400 w-full")
let fondoOp2 = ref("text-center bg-white w-full")
function cambiarColor() {
  if(checked.value){
    fondoOp1.value = "text-center bg-white w-full";
    fondoOp2.value = "text-center bg-blue-400 w-full";
    console.log(fondoOp1.value);
  }else{
    fondoOp1.value = "text-center bg-blue-400 w-full";
    fondoOp2.value = "text-center bg-white w-full";
    console.log(fondoOp1.value);
  }
}

</script>
