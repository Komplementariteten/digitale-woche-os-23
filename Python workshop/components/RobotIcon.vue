<script setup lang="ts">
import { ref } from 'vue'

let iconIndex = ref(0);

let intervalId = setInterval(function() {
    iconIndex.value = (iconIndex.value + 1) % 4;
}, 1000);


</script>

<style>

  .icon {
    -webkit-filter: drop-shadow(5px 5px 5px #000);
    filter: drop-shadow(5px 5px 5px #000);
  }

  .angry {
    color: red;
  }

  .confused {
    color: cyan;
  }

  .dead {
    color: greenyellow;
  }

  .normal {
    color: white;
  }
</style>

<template>
  <mdi-robot-angry-outline class="text-5xl angry icon" v-if="iconIndex == 0"/>
  <mdi-robot-confused-outline class="text-5xl confused icon" v-if="iconIndex == 1"/>
  <mdi-robot-outline class="text-5xl normal icon" v-if="iconIndex == 2"/>
  <mdi-robot-dead-outline class="text-5xl dead icon" v-if="iconIndex == 3"/>
</template>
