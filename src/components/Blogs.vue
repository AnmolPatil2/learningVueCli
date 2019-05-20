<template>
  <div class="Blogs">
    <h1>Blogs</h1>
    <div v-for="data in data" :key="data.id">
      <p>{{data.title}}</p>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  name: "Blogs",
  data() {
    return {
      data: []
    };
  },
  props: {},
  created() {
    axios.get("https://jsonplaceholder.typicode.com/todos").then(Response => {
      console.log(Response);
      this.data = Response.data;
    });
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>
