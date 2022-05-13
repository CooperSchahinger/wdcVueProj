<template>
  <div class="event-details">
    <h1>Event Details</h1>
    <h2>Contains Detials from Event Database</h2>
  </div>
</template>

<style scoped>
.event-details {
  height: 100vh;
}

h1,
h2 {
  color: #fefae0;
}
</style>

<script>
export default {
  props: {
    event: {
      type: Object,
      required: true,
    },
  },
};
</script>
