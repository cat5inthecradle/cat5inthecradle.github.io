<template>
  <section>
    <h1 class="">All-State Schedule</h1>
    <event-list/>
  </section>
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
