<template>
  <div id="events" class="offset">
    <div class="jumbotron">
      <div class="header text-center">Our Events</div>
      <div class="narrow text-center">
        <div class="row text-center">
          <div class="col-md-4">
            <Card title="Learn about working remotely" image="step1.png">
              <p>Get a full overview of Toptal advantages and learn how to start.</p>
            </Card>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import Card from "./Card.vue";

export default {
  name: "EventsSection",
  components: {
    Card,
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
