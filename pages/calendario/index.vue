<template>
  <div class="container">
    <h1 class="h1-responsive">Calendario Distrital</h1>
    <hr />
    <FullCalendar
      defaultView="dayGridMonth"
      googleCalendarApiKey="AIzaSyCQ9aa3u8WaaIwL_93ZkYqEWoKgaWEE1Gk"
      :eventSources="[
        { googleCalendarId: 'd7oe15ml0vft4sqs9ohnu724es@group.calendar.google.com'},
        { googleCalendarId: 'zona9.org.ar_6fgl3k2ddd0jfg589e8cejtpms@group.calendar.google.com', className: 'success-color'}
      ]"
      :plugins="calendarPlugins"
    />

    <hr />
    <h4>Link a Google Calendar</h4>
    <hr />
    <a
      class="btn waves-light success-color white-text"
      href="https://calendar.google.com/calendar/embed?src=d7oe15ml0vft4sqs9ohnu724es%40group.calendar.google.com&ctz=America%2FArgentina%2FBuenos_Aires"
    >Ir a google Calendar del Distrito</a>
        <a
      class="btn waves-light info-color white-text"
      href="https://calendar.google.com/calendar/embed?src=zona9.org.ar_6fgl3k2ddd0jfg589e8cejtpms%40group.calendar.google.com&ctz=America%2FArgentina%2FBuenos_Aires"
    >Ir a google Calendar de la zona</a>
  </div>
</template>
    
<style lang='scss'>
@import "@fullcalendar/core/main.css";
@import "@fullcalendar/daygrid/main.css";
</style>
<script>
//https://github.com/Wanderxx/vue-fullcalendar
//https://fullcalendar.io/docs/vue
import FullCalendar from "@fullcalendar/vue";
import dayGridPlugin from "@fullcalendar/daygrid";
import googleCalendarPlugin from "@fullcalendar/google-calendar";

export default {
  components: {
    FullCalendar // make the <FullCalendar> tag available
  },

  head() {
    return {
      title: "Calendario Distrital"
    };
  },
  data() {
    return {
      calendarPlugins: [dayGridPlugin, googleCalendarPlugin]
    };
  }
};
</script>
</script>
