<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld
  },
  created() {
    fetch("https://sheetdb.io/api/v1/org6l4fy7fwm9").then(v => {
      console.log(v);
    });
  }
};
</script>
