<template>
  <!-- dimensiones, margin y padding, display, elementos visuales (cursor pointer), asignación de colores -->
  <div 
    class="w-48 flex justify-center border-2 rounded-xl cursor-pointer border-blue-800" 
    @click="activarRadio"
  >
    <div class="w-full text-center rounded-l-md" :class="{ 'bg-blue-800 text-white': checked }">
      <p>{{ option1 }}</p>
    </div>
    <input class="hidden" type="radio" :checked="checked" />
    <div class="w-full text-center rounded-r-md" :class="{ 'bg-blue-800 text-white': !checked }">
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

/* const fnFlecha = () => {}*/

const checked = ref(true);
function activarRadio() {
  if (checked.value) {
    checked.value = false;
  } else {
    checked.value = true;
  }
  console.log(checked.value)
}
</script>
