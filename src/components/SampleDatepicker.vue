<script>
import VueDatePicker from '@vuepic/vue-datepicker';
import '@vuepic/vue-datepicker/dist/main.css'

export default {
  compatConfig: {
        MODE: 3,
        COMPONENT_ASYNC: false
    },
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
  v-model:value="date"
  format="YYYY-MM-DD"
  type="date"
  placeholder="Select date"
  >
  </VueDatePicker>
</template>
