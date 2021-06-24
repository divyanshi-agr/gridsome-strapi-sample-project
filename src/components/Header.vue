<template>
  <div>
    <h1>{{ title }}</h1>
    <p>{{ date }}</p>
    <img :src="img" alt="Header img" />
  </div>
</template>

<script>
export default {
  props: {
    id: String,
    title: String,
    date: String,
    img: String,
  },
};
</script>

<style></style>
