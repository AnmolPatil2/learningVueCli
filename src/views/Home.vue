<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">

    <Navbar></Navbar>

    <Profile></Profile>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import Navbar from "@/components/Navbar";
import Blogs from "@/components/Blogs";
import Profile from "@/components/Profile";
export default {
  name: "home",
  components: {
    HelloWorld,
    Navbar,
    Blogs,
    Profile
  }
};
</script>
