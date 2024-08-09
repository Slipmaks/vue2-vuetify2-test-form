<template>
  <v-app>
    <div class="background-section">
      <div
        class="gradient-section d-flex align-center justify-center"
      >
        <Form />
      </div>
    </div>
  </v-app>
</template>

<script>
import Form from "./components/Form";

export default {
  name: "App",

  components: {
    Form,
  },

  data: () => ({
    //
  }),
};
</script>
<style>
.background-section {
  background-color: black;
}
.gradient-section {
  width: 100%;
  min-height: 100vh;
  background: radial-gradient(circle at left top, #fafafa30, transparent 50%),
    radial-gradient(circle at right bottom, #fafafa30, transparent 50%);
}
</style>
