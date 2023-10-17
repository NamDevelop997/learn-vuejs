<template>
  <div>
    <ul>
      <li style="list-style: none;">
        <p>{{ user.id }} - {{ user.email }}</p></li>
    </ul>
  </div>
</template>
<script>
export default {
  data() {
    return {};
  },
  props: {
    user: {
      type: Object,
      default: {},
    },
  },
};
</script>
<style></style>
