<template>
  <div>
    <h1>List user</h1>
    <User v-for="(item,index) in listUser" :key="index" :user="item"/>
  </div>
</template>
<script>
import User from "./User.vue";
export default {
  data() {
    return {
      // users: [],
    };
  },
  props: {
    listUser: {
      type: Array,
      default: [],
    },
  },
  components: {
    User,
  },
};
</script>
<style></style>
