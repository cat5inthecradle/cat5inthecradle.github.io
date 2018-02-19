<template>
  <div>
    <section>
      <h1>All-State Schedule</h1>
      <event-list/>
    </section>
    <br>
    <section>
      <h1>Emergency Contacts</h1>
      <div class="contact-list">
        <a v-for="contact in contacts" :key="contact.name" class="button button-pill button-primary" :href="'tel:'+contact.tel">{{ contact.name }}</a>
      </div>
    </section>
  </div>
</template>

<script>
import EventList from "./event-list"
export default {
  layout: "simple-dark",
  components: { EventList },
  data() {
    return {
      contacts: [
        { name: "Darin Webb", tel: "+17069694420" },
        { name: "Amanda Pichler", tel: "+15156697404" }
      ]
    }
  }
}
</script>

<style lang="scss">
.container {
  margin-top: 1em;
}

h1,
h2,
h3,
h4 {
  width: 100%;
  text-align: center;
}

.contact-list > * {
  margin: auto;
  width: 12em;
  display: block;
  margin-bottom: 2em;
}
</style>
