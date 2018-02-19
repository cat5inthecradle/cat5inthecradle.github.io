<template>
  <div>
    <main>
      <nuxt />
    </main>
    <footer>
      <p>Copyright 2018 IHSSA</p>
    </footer>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
@import "../node_modules/normalize.css/normalize.css";

body {
  background-color: #ededed;
  background-image: url("../assets/concrete_seamless.png");
  color: #2b2b2b;

  font-family: "Bree Serif", serif;
}

.main {
  padding-left: 1em;
  padding-right: 1em;
}

footer {
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 3em;
  background-color: rgb(46, 46, 46);
  background-image: url("../assets/dark-triangles.png");
  color: #ededed;
  padding-right: 1em;
  padding-left: 1em;
  display: flex;
  justify-content: left;
  align-content: middle;
}
</style>
