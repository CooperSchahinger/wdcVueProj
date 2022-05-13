<template>
  <div class="nav-container">
    <h1 v-on:click="routeHome()" class="app-name">Application name</h1>
    <div class="nav-items-container">
      <ul class="nav-items">
        <router-link class="nav-item" to="/">Home</router-link>
        |
        <router-link class="nav-item" to="/about">About</router-link>
        |
        <router-link class="nav-item" to="/events">Events</router-link>

        <router-link class="nav-item-login" to="/login">
          <div class="button">Login</div>
        </router-link>

        <router-link class="nav-item" to="/signup">
          <div class="button">Sign-up</div>
        </router-link>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    routeHome() {
      this.$router.push({ name: "Home" });
    },
  },
};
</script>

<style scoped>
.nav-container {
  display: inline-flex;
  width: 100vw;
  padding-left: 0.75vw;
  background-color: #283618;
  color: #fefae0;
}

.app-name {
  padding: 10px;
  color: #fefae0;
}
.nav-items-container {
  padding-top: 1.5vh;
}

.button {
  width: 5vw;
  padding: 10px;
  color: #fefae0;
}
.nav-item {
  padding: 10px;
  color: #fefae0;
}

.nav-item-login {
  /* text-aligns: right; */
  padding: 10px;
  margin-left: 55vw;
  color: #fefae0;
  /* margin-left: 80vw; */
}
</style>
