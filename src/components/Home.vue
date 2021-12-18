<template>
  <!-- <h4>Email {{ email }}</h4>

  <h4>name {{ getName() }}</h4>
  <h4>id {{ getID() }}</h4>
  <h3>All Data {{ getData() }}</h3> -->
  <h4 v-on:mousemove="getConsole">Home components</h4>
  <button v-on:click="getData('button 1 clicked')">Click me</button>
  <button v-on:dblclick="getData('button dubble clicked')">Click me</button>
</template>

<script>
export default {
  name: "Home",
  methods: {
    getData(data) {
      alert(data);
    },
    getConsole(){
        console.warn("function called");
    }
  },
  //   data() {
  //     return {
  //       email: "toma@effat.com",
  //       //function
  //       getName: function () {
  //         return "toma";
  //       },
  //     };
  //   },
  //   //multipal function
  //   methods: {
  //     getID() {
  //       return "1";
  //     },
  //     getData() {
  //       return {
  //         fullName: "effat",
  //         Address: "Dhaka",
  //         email: this.email,
  //       };
  //     },
  //   },
};
</script>

<style scoped>
h1 {
  color: red;
}
</style>
