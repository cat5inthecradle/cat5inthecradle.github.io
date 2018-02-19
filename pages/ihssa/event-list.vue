<template>
  <div>
    <div class="schedule-row" v-for="event in schedule" :key="event.title">
      <div class="col-1 time">{{ event.time }}</div>
      <div class="col-grow title">{{ event.title }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "EventList",
  data() {
    return {
      schedule: [
        { time: "9:25", title: "Hunchback (MT)" },
        { time: "10:12", title: "Yo-Yo Man (SM)" },
        { time: "10:40", title: "A Murder of Crows (RT)" },
        { time: "11:18", title: "Artemis (SM)" },
        { time: "11:34", title: "Opus Siderum (SM)" },
        { time: "11:50", title: "Perspectives (TV)" },
        { time: "12:35", title: "Face Stealer (GM)" },
        { time: "1:35", title: "Leaving Iowa (OA)" },
        { time: "2:08", title: "AIR (RN)" },
        { time: "2:58", title: "Brunch Bunch (TV)" },
        { time: "3:29", title: "Faithful Elephants (CR)" }
      ]
    }
  }
}
</script>

<style>
.schedule-row {
  display: flex;
  margin: auto;
  margin-bottom: 0.333em;
  max-width: 450px;
}

.time {
  display: block;
  width: 5em;
  text-align: left;
  padding: 0 0.5em;
  text-align: left;
}

.title {
  display: block;
  flex-grow: 1;
  padding: 0 0.5em;
  text-align: right;
}
</style>
