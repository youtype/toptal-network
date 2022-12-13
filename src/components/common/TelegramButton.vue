<template>
  <a :href="telegramLink" target="_blank" class="btn btn-outline-light btn-lg">
    Join our Telegram chat
  </a>
</template>
<script>
import { TELEGRAM_LINK } from "@/constants.js";

export default {
  name: "TelegramButton",
  data() {
    return {
      telegramLink: TELEGRAM_LINK,
    };
  },
};
</script>
