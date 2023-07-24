<script>
import VueDatePicker from '@vuepic/vue-datepicker';
import '@vuepic/vue-datepicker/dist/main.css'

export default {
  components: {
    VueDatePicker
  },
  data() {
    return {
      date: new Date(),
    };
  }
}
</script>

<template>
  <h1>Playground</h1>

  <VueDatePicker
  placeholder="Type a date..."
  :enable-time-picker="false"
  format="MM/dd/yyyy"
  position="center"
  :dark="false"
  v-model="date"
  >
  </VueDatePicker>
</template>
