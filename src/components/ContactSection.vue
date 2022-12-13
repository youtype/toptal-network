<template>
  <div id="contact" class="offset">
    <footer>
      <div class="button-wrapper">
        <TelegramButton />
      </div>
      <div class="logo-wrapper">
        <img src="@/assets/images/logo.png" />
      </div>
    </footer>
  </div>
</template>
<script>
import TelegramButton from "./common/TelegramButton.vue";

export default {
  name: "ContactSection",
  components: {
    TelegramButton,
  },
};
</script>
<style scoped>
#contact:before {
  display: block;
  content: "";
  height: 1.6rem;
  margin-top: -1.6rem;
}
.button-wrapper {
  margin: 1rem 0 0.5rem;
  text-align: center;
}
footer {
  color: white;
  padding: 0.7rem 0;
}
.logo-wrapper {
  text-align: end;
}
.logo-wrapper img {
  height: 40px;
  border-radius: 100%;
  margin: 0 1rem;
}
footer a {
  color: white;
}
</style>
