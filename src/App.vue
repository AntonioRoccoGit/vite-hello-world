<script>
import AppTitle from "./components/AppTitle.vue";
import AppJumbotron from "./components/AppJumbotron.vue";
import EmojPicker from "./components/EmojPicker.vue";

export default {
  components: {
    AppTitle,
    AppJumbotron,
    EmojPicker
  },
  data() {
    return {

    }
  }
}
</script>

<template>
  <AppTitle />
  <AppJumbotron />
  <EmojPicker />
</template>

<style></style>