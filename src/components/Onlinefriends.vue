<template>
  <div id="allfriends">
    <h2>Allfriends</h2>
    <div v-for="(friend,index) in friends" :key="index">
      <p v-if="friend.online" @click="f1(friend.name)">{{friend.name}}</p>
    </div>
    <Onlinefriends :friends="friends"/>
  </div>
</template>
<script>
export default {
  name: "Allfriends",
  props: ["friends"],
  data() {
    return {};
  },
  methods: {
    f1(name) {
      console.log("hii");
      this.$emit("delete", { name });
    }
  }
};
</script>
