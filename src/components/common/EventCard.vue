<template>
  <Card :title="title" :image="image || 'step1.png'">
    <p>{{ dateLocal }} ({{ dateRelative }})</p>
    <slot />
    <p v-if="telegram"><TelegramButton /></p>
  </Card>
</template>
<script>
import Card from "./Card.vue";
import dayjs from "dayjs";
import timezone from "dayjs/plugin/timezone";
import utc from "dayjs/plugin/utc";
import { TELEGRAM_LINK } from "@/constants.js";
import relativeTime from "dayjs/plugin/relativeTime";
import TelegramButton from "./TelegramButton.vue";

dayjs.extend(utc);
dayjs.extend(timezone);
dayjs.extend(relativeTime);

export default {
  name: "EventCardComponent",
  components: {
    Card,
    TelegramButton,
  },
  data() {
    return {
      telegramLink: TELEGRAM_LINK,
    };
  },
  props: {
    title: {
      type: String,
      required: true,
    },
    date: {
      type: String,
      required: true,
    },
    image: {
      type: String,
      required: false,
    },
    telegram: {
      type: Boolean,
      required: false,
    },
  },
  computed: {
    dateRaw() {
      return dayjs(this.date).tz("Europe/Istanbul");
    },
    dateLocal() {
      return this.dateRaw.format("MMM D, YYYY hh:mm");
    },
    dateRelative() {
      return this.dateRaw.fromNow();
    },
  },
};
</script>
<style scoped></style>
