<template>
  <div v-on:click="activarRadio"
    class="flex border-black bg-white justify-center rounded-md overflow-hidden cursor-pointer">
    <div class="text-center w-full" :class="{ 'bg-blue-600 text-white': checked }">
      <p>{{ option1 }}</p>
    </div>
    <input class="" type="radio" :checked="checked" />
    <div class="text-center w-full" :class="{ 'bg-blue-600 text-white': !checked }">
      <p>{{ option2 }}</p>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const props = defineProps({
  option1: {
    type: String,
    default: "option1"
  },
  option2: {
    type: String,
    default: "option2"
  }
});

let checked = ref(true);
function activarRadio() {
  if (checked.value) {
    checked.value = false;
  } else {
    checked.value = true;
  }
  console.log(checked.value)
}

let fondoOp1 = ref("bg-blue-400")
let fondoOp2 = ref("bg-white")
function cambiarColor() {
  if (checked.value) {
    fondoOp1.value = "bg-white";
    fondoOp2.value = "bg-blue-400";
    console.log(fondoOp1.value);
  } else {
    fondoOp1.value = "bg-blue-400";
    fondoOp2.value = "bg-white";
    console.log(fondoOp1.value);
  }
}
</script>
