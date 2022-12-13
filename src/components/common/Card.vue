<template>
  <div>
    <img v-if="image" :src="imageSrc" :alt="title" />
    <div class="description">
      <h3>{{ title }}</h3>
      <slot />
    </div>
  </div>
</template>
<script>
export default {
  name: "CardComponent",
  props: {
    title: {
      type: String,
      required: true,
    },
    image: {
      type: String,
      required: false,
    },
  },
  computed: {
    imageSrc() {
      return require(`@/assets/images/${this.image}`);
    },
  },
};
</script>
<style scoped>
h3 {
  font-size: 1.3rem;
  text-transform: uppercase;
  padding-bottom: 0.4rem;
}
p {
  font-size: 1.1rem;
}
img {
  width: 100%;
}
.description {
  margin: 25px 0;
}
</style>
