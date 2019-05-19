<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">

    <Navbar></Navbar>
    <Allfriends/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import Navbar from "@/components/Navbar";
import Allfriends from "@/components/Allfriends";
import Onlinefriends from "@/components/Onlinefriends";
export default {
  name: "home",
  components: {
    HelloWorld,
    Navbar,
    Onlinefriends,
    Allfriends
  }
};
</script>
