<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">

    <Navbar></Navbar>
    <Blogs></Blogs>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import Navbar from "@/components/Navbar";
import Blogs from "@/components/Blogs";
export default {
  name: "home",
  components: {
    HelloWorld,
    Navbar,
    Blogs
  }
};
</script>
