<template>
  <div>
    <h1>Im the headerrr</h1>
    <h2>ID: {{ id }}</h2>
    <p><b>Title:</b> {{ title }}</p>
    <p><b>Date:</b> {{ date }}</p>
    <img :src="img" alt="Header img" />
    <p>I am inside the header</p>
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
