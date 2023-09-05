<template>
  <div id="app">
    <cb-login />
  </div>
</template>

<script>
import Vue from "vue";
import Component from "vue-class-component";
import Login from "./components/Login";
// import StarRating from "./components/StarRating";

// Define the component in class-style
@Component({
  name: "app",
  props: [
    "name",
    "displayLabel",
    "disabled",
    "value",
    "fieldDesc",
    "placeholder",
    "focus",
    "customClass",
    "required",
    "fluid",
    "noValidationOnBlur",
    "isMultiDecimalField",
  ],
  components: {
    "cb-login": Login,
  },
})
export default class App extends Vue {
  // Class properties will be component data
  count = 0;

  // Methods will be component methods
  increment() {
    this.count++;
  }

  decrement() {
    this.count--;
  }
}
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: #131319;
  /* width: 100%; */
  height: 100vh;
}
</style>
