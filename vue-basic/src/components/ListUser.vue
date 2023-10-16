<template>
  <div>
    <h1>List user</h1>
    <!-- <user></user> -->
    <User/>
  </div>
</template>
<script>
import User from "./User.vue";
export default {
  data() {
    return {
      users: [],
    };
  },
  components: {
    User,
  },
};
</script>
<style></style>
