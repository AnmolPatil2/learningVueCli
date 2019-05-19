<template>
  <div id="allfriends">
    <h2>Allfriends</h2>
    <div v-for="(friend,index) in friends" :key="index">
      <span v-if="friend.online">{{friend.name}}</span>
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
  }
};
</script>
