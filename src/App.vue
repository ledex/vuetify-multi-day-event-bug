<template>
  <v-app>
    <v-main>
      <v-calendar :events="events"/>
      The event does not span across the entire duration, but is present twice, on the start date and end date.
    </v-main>
  </v-app>
</template>

<script setup lang="ts">
const events = [
  {
    title: `Green event`,
    start: new Date('2024-01-10 00:00'),
    end: new Date('2024-01-15 23:59'),
    allDay: false,
    color: 'green'
  },
]
</script>
