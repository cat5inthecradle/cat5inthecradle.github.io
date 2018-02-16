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
        { time: "05:00", title: "Wake Up" },
        { time: "06:45", title: "Load Buses" },
        { time: "5:30 - 6:15am", title: "Breakfast & Wristbands" },
        { time: "6:30am", title: "Bus leaves, bring everything!" },
        { time: "6:40am", title: "Truck unloads Choral at CY" },
        { time: "7:00am", title: "Truck unloads Readers at Scheman" },
        { time: "7:15am", title: "Banner Carriers report to CY stage" },
        { time: "7:20am", title: "DEREK return wristbands & get programs from Scheman" },
        { time: "7:30am", title: "Hand out programs & orange flags" },
        { time: "8:00am", title: "OPENING CEREMONIES" },
        { time: "8:15am", title: "Musical Theatre commute to Ames Auditorium" },
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