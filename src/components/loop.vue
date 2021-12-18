<template>
  <h1>Loop</h1>
  <ul>
    <li v-for="item in technology" :key="item">{{ item }}</li>
  </ul>
  <br />

  <ul>
    <li v-for="item in user" : key="item.email">
      Name is :{{ item.name }} and email is : {{ item.email }}
    </li>
  </ul>
</template>

<script>
export default {
  name: "loop",
  data() {
    return {
      technology: ["java", "php", "js", "python"],
      //array of object
      user: [
        {
          name: "toma",
          email: "toma@gmail.com",
          phone: "017",
        },

        {
          name: "t",
          email: "t@gmail.com",
          phone: "017",
        },
      ],
    };
  },
};
</script>

<style scoped>
h1 {
  color: red;
}
</style>
