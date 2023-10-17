<script>
import ListUser from "./components/ListUser.vue";
export default {
  data() {
    return {
      message:"hello world",
      listUser: [
        {id:1, email:"gmail1.com", active:false},
        {id:2, email:"gmail2.com", active:true},
        {id:3, email:"gmail3.com", active:false},
        {id:4, email:"gmail4.com", active:true},
        {id:5, email:"gmail5.com", active:true},
        {id:6, email:"gmail6.com", active:false},
      ]
    }
  },
  components: {
    ListUser
  }
}
</script>

<template>
  <header>
    <list-user :message="message" :listUser="listUser "/>
  </header>

  <main></main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
