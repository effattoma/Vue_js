<template>
  <HelloWorld msg="Practice Project" />
<!-- <loop /> -->
  <!-- <condition /> -->
  <parentAndChild />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import parentAndChild from "./components/parentAndChild.vue";
// import loop from "./components/loop.vue";
// import condition from "./components/condition.vue"
// import TwoWayBinding from "./components/TwoWayBinding.vue";
export default {
  name: "App",
  components: {
    HelloWorld,
    parentAndChild
    // loop,
// condition,
    // TwoWayBinding,
  },
};
</script>
