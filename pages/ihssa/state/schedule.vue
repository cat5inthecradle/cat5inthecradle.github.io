<template>
  <section>
    <table>
      <thead>
        <tr>
          <th>#</th>
          <th>Time</th>
          <th>School</th>
          <th>Title</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>1</td>
          <td>8:00</td>
          <td>132</td>
          <td>Opus Siderum: Work of the Stars</td>
        </tr>
      </tbody>
    </table>
  </section>
</template>

<script>
export default {
  data() {
    return {
      events: [
        {
          time: "8:00",
          school: "132",
          title: "Opus Siderum: Work of the Stars"
        },
        {
          time: "8:10",
          school: "498",
          title: "Artemis and the Dragon: The Solen Child"
        },
        {
          time: "8:00",
          school: "602",
          title: "Yo-Yo Man: A Life on the Line (And He Gets the Girl)"
        }
      ]
    }
  }
}
</script>
