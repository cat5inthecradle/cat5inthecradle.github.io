<template>
  <section>
    <h2>Schedule</h2>
    <div v-for="event in schedule" class="schedule-grid">
        <span class="col-1 time">{{ event.time }}</span>
        <span class="col-grow title">{{ event.title }}</span>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'event-list',
  data() {
    return {
      schedule: [
        { time: "9:25", title: "hunchback MT" },
        { time: "12:10", title: "Yo-Yo Man SM" },
        { time: "10:40", title: "A Murder of Crows RT" },
        { time: "11:18", title: "Artemis SM" },
        { time: "11:34", title: "Opus Siderum SM" },
        { time: "11:50", title: "Perspectives TV" },
        { time: "12:35", title: "Face Stealer GM" },
        { time: "1:35", title: "Leaving Iowa OA" },
        { time: "2:08", title: "AIR RN" },
        { time: "2:58", title: "Brunch Bunch TV" },
        { time: "3:29", title: "Faithful Elephants CR" },
      ],
    }
  },
}
</script>

<style>

.schedule-grid {
  display: flex;
  margin-bottom: .333em;
}

.time {
  display: block;
  width: 10em;
  text-align: left;
  padding: 0 .5em;  
}

.title {
  display: block;
  flex-grow: 1;
  padding: 0 .5em;
}

</style>