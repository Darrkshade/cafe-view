<template>
  <div class="app">
    <NavigationBar />
    <router-view />
  </div>
</template>

<script>
import NavigationBar from "@/components/NavigationBar.vue";

export default {
  name: "App",
  components: {
    NavigationBar
  }
};
</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
  font-family: "Roboto Regular";
}

html,
body {
  min-height: 100vh;
  width: 100vw;
}

.app {
  height: 100vh;
  width: 100vw;
  background-image: url("./assets/background.jpg");
  background-size: 100% 100%;
}
</style>
