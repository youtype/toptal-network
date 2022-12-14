<template>
  <div id="events" class="offset">
    <div class="jumbotron">
      <div class="header text-center">Our Events</div>
      <div class="narrow text-center">
        <div class="row text-center">
          <div class="col-md-4">
            <EventCard title="Project presentation" date="2022-12-17 16:30:00" telegram>
              <p>Project presentation at Legat Business forum.</p>
              <p>Address: Denizim Park Antalya</p>
            </EventCard>
          </div>
          <div class="col-md-4">
            <EventCard title="Project presentation" date="2022-12-18 16:30:00" telegram>
              <p>Project presentation at Legat Business forum.</p>
              <p>Address: Denizim Park Antalya</p>
            </EventCard>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import EventCard from "./common/EventCard.vue";

export default {
  name: "EventsSection",
  components: {
    EventCard,
  },
};
</script>
<style scoped>
.jumbotron {
  background-color: #1b45b1;
  color: white;
}
.header {
  font-size: 3rem;
}
img {
  width: 100%;
}
#features .narrow {
  padding-top: 0;
  background-color: #101010;
}
#features:before {
  background-color: #101010;
  display: block;
  content: "";
  height: 3.7rem;
  margin-top: -3.7rem;
}
</style>
