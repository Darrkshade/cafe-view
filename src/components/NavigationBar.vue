<template>
  <nav class="navbar">
    <img class="navbar-logo" :src="logo" alt="Cafe Logo" />
    <div class="navbar-link-container">
      <router-link class="navbar-link" to="#">Home</router-link>
      <router-link class="navbar-link" to="#">About</router-link>
      <router-link class="navbar-link" to="#">Menu</router-link>
      <router-link class="navbar-link" to="#">Contact</router-link>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavigationBar",
  data: () => ({
    logo: require("../assets/logo.png")
  })
};
</script>

<style scoped lang="scss">
.navbar {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  width: 100%;
  background: #ddb892;

  &-logo {
    height: 75px;
    width: 175px;
  }

  &-link {
    color: white;
    text-decoration: none;
    font-size: 2rem;
    margin: 0 1rem;

    &-container {
      display: flex;
      flex-direction: row;
      align-items: center;
      margin: 0 auto;
    }
  }
}
</style>
