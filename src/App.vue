<template>
  <div id="app">
    <MySwiper :mediaItems="mediaItems" />
  </div>
</template>

<script>
import MySwiper from "./components/MySwiper";

export default {
  name: "App",
  components: {
    MySwiper,
  },
  data() {
    return {
      mediaItems: Array(30)
        .fill()
        .map((x, i) => `https://placekitten.com/100/${100 + i}`),
    };
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
