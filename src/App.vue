<template>
  <div id="app">
    <HomeSection />
    <GoalSection />
    <EventsSection />
    <ContactSection />
  </div>
</template>

<script>
import HomeSection from "./components/HomeSection.vue";
import GoalSection from "./components/GoalSection.vue";
import EventsSection from "./components/EventsSection.vue";
import ContactSection from "./components/ContactSection.vue";
export default {
  name: "app",
  components: {
    HomeSection,
    GoalSection,
    EventsSection,
    ContactSection,
  },
};
</script>
<style>
html {
  scroll-behavior: smooth;
}
body {
  font-family: Roboto -apple-system, BlinkMacSystemFont, "Segoe UI", Oxygen, Ubuntu,
    Cantarell, "Open Sans", "Helvetica Neue", sans-serif !important;
  overflow-x: hidden;
  color: #505962;
  background-color: #101010;
  font-family: "Noto Sans", sans-serif;
}
.offset:before {
  display: block;
  content: "";
  height: 4rem;
  margin-top: -4rem;
}
.narrow {
  width: 75%;
  margin: 1.5rem auto;
  padding-top: 2rem;
}
.narrow h1 {
  font-size: 2.4rem;
}
.jumbotron {
  margin-top: 0;
  margin-bottom: 0;
  padding: 2rem 0 3.5rem;
  border-radius: 0;
}
.btn-lg {
  border-width: medium;
  border-radius: 10px;
  padding: 0.6rem 1.3rem;
  font-size: 1.1rem;
}
.btn-secondary {
  border-width: medium;
  border-radius: 0;
  text-transform: uppercase;
  font-size: 1.2rem;
  padding: 0.6rem 1.2rem;
  margin: 1rem;
  color: white !important;
  background-color: #1b45b1;
  border-color: #1b45b1;
  border-radius: 10px;
}
.btn-md {
  border-radius: 2rem;
}
.btn-lg:hover,
.btn-secondary:hover {
  background-color: #1b45b1;
  border-color: #1b45b1;
  color: white;
}
h3.heading {
  font-size: 1.9rem;
  font-weight: 700;
  text-transform: uppercase;
  /* margin-bottom: 1.9rem; */
}
.heading-underline {
  width: 12rem;
  height: 0.2rem;
  background-color: #204ecf;
  margin: 0 auto 2rem;
}
</style>
