<template>
  <section>
    <h1>
      IHSSA State Contest
    </h1>
    <p>
      at West Des Moines Valley High School
    </p>
    <ul class="contest-links">
      <li><a href="/ihssa/state/schedule">Schedule</a></li>
      <li><a href="/ihssa/state/map">Map</a></li>
      <li><a href="/ihssa/state/faq">FAQ</a></li>
      <li><a href="/ihssa/state/contact">Contact</a></li>
    </ul>
  </section>
</template>
<script>
export default {
  name: "State",
  layout: "ihssa"
}
</script>
<style>
ul.contest-links {
  list-style: none outside none;
  padding: 0;
}

ul.contest-links > li {
  text-align: center;
}
</style>
