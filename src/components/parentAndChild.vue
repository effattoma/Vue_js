<template>
  <h1>Pass data to child Component</h1>
  <child name="Effat Tamanna" :user="user" :getData="getData" />
</template>

<script>
import child from "./child.vue";
export default {
  name: "parentAndChild",
  components: {
    child,
  },
  data() {
    return {
      user: { name: "toma", email: "effat@gmail.com" },
    };
  },

  methods: {
    getData() {
      console.warm("parent function called");
      atert("hello");
    },
  },
};
</script>
