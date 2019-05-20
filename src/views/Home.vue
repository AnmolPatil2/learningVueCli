<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">

    <Navbar></Navbar>
    <ul>
      <li v-for="(id,index) in ids " :key="index">
        <router-link :to="{name:'Profile',params:{name:id}}">{{id}}</router-link>
      </li>
    </ul>
    <button @click="GoHome">Go Home</button>
    <button @click="goFront">Go Home</button>
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
  },
  data() {
    return {
      ids: ["1", "2", "3", "4"]
    };
  },
  methods: {
    GoHome() {
      this.$router.push({ name: "about" });
    },
    goFront() {
      this.$router.go(-1);
    }
  }
};
</script>
