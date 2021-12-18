<template>
  <h1>Condition</h1>
  <h2 v-if="show">If Else Condition</h2>
  <h2 v-else>Else Condition</h2>
  <button v-on:click="show=!show">Toogle</button>
</template>

<script>
export default {
  name: "condition",
  data() {
    return {
      show: false,
    };
  },
};
</script>
