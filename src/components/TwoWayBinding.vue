<template>
  <h1>Two Way Binding</h1>
  <h4>Get checkbox and Redio button values</h4>

  <h5>technology</h5>
  <level for="java"> Java </level>
  <input type="checkbox" value="java" id="java" v-model="technology" />

  <level for="php"> PHP </level>
  <input type="checkbox" value="php" id="php" v-model="technology" />

  <level for="js"> JS </level>
  <input type="checkbox" value="js" id="js" v-model="technology" />

  <br />
  <br />

  <h3>Who I am</h3>
  <level for="student">Student</level>
  <input type="radio" name="who" id="student" v-model="who" value="student" />

  <level for="developer">Developer</level>
  <input type="radio" name="who" id="developer" v-model="who" value="developer" />
  <h4>Selected technology: {{ technology }}</h4>
  <h3>I am a : {{ who }}</h3>
  <!-- <input type="text" v-model="count" />
  <h3>{{count}}</h3> -->

  <!-- <input type="text" placeholder="email" v-model="email" />
  <br />
  <input type="password" placeholder="password"  v-model="password"/>
  <br />
  <button v-on:click="getData" type="button">Get Values</button> -->
</template>

<script>
export default {
  name: "TwoWayBinding",

  data() {
    return {
      technology: [],
      who: null,
    };
  },
  //  data(){
  //      return {
  //          count:10
  //      }
  //  }

  // data(){
  //     return{
  //         email: null,
  //         password: null,
  //     }
  // },
  // methods:{
  //     getData(){
  //         console.warn("values : ",this.email , this.password);
  //     }
  // }
};
</script>
