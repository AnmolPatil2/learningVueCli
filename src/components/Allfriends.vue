<template>
  <div id="allfriends">
    <h2>Allfriends</h2>
    <div v-for="(friend,index) in friends" :key="index">
      <span>{{friend.name}}</span>
    </div>
    <Onlinefriends :friends="friends"/>
  </div>
</template>
<script>
import Onlinefriends from "./Onlinefriends";
export default {
  name: "Allfriends",
  components: {
    Onlinefriends
  },

  data() {
    return {
      friends: [
        {
          name: "mango",
          online: true
        },
        {
          name: "mango1",
          online: false
        },
        {
          name: "mango2",
          online: false
        },
        {
          name: "mango3",
          online: true
        }
      ]
    };
  }
};
</script>
