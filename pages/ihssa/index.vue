<template>
  <div class="container">
    <header>
      <h1 class="">IHSSA All-State Contest</h1>
      <p class="lead">West Des Moines Valley High School</p>
    </header>
    <main>
      <event-list/>
    </main>
  </div>
</template>

<script>
import EventList from "./event-list"
export default {
  layout: "ihssa",
  components: { EventList }
}
</script>

<style lang="scss">
.container {
  margin-top: 1em;
}
</style>
