<template>
  <div class="Profile">
    <h1>Profiles for {{var1}}</h1>
  </div>
</template>

<script>
export default {
  name: "Profile",
  props: {},
  data() {
    return {
      var1: this.$route.params.name
    };
  },
  methods: {
    f1() {
      this.var1 = this.$route.params.name;
    }
  },
  watch: {
    $$route: "f1"
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>
