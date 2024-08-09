<template>
  <v-form class="register-form pt-13 px-8 my-13">
    <div class="d-flex flex-column align-center mb-8 gradient-text">
      <h3 class="mb-2 text-h4">Sing Up for Free</h3>
      <p class="mb-0 grey--text">Welcome, let's het to know each other!</p>
    </div>
    <div class="mb-5">
      <p class="mb-2">Full name</p>
      <v-text-field
        placeholder="Enter your full name"
        outlined
        color="#CCCCCC"
        class="rounded-lg"
        background-color="#27272926"
        dense
        hide-details
        filled
        height="48"
        autocomplete="name"
      ></v-text-field>
    </div>
    <div class="mb-5">
      <p class="mb-2">Email</p>
      <v-text-field
        placeholder="Enter your email"
        height="48"
        hide-details
        color="#CCCCCC"
        class="rounded-lg"
        background-color="#27272926"
        dense
        filled
        outlined
        autocomplete="email"
      ></v-text-field>
    </div>
    <div class="mb-8">
      <p class="mb-2">Phone number</p>
      <v-text-field
        class="rounded-lg"
        placeholder="Enter your phone number"
        height="48"
        color="#CCCCCC"
        background-color="#27272926"
        hide-details
        dense
        filled
        outlined
        autocomplete="tel"
      ></v-text-field>
    </div>
    <div class="mb-12">
      <v-btn width="100%" x-large class="mb-5 black--text rounded-lg white"
        >Continue</v-btn
      >
      <v-btn width="100%" class="rounded-lg white--text border" outlined x-large
        >I have an account</v-btn
      >
    </div>
    <p class="text-center text-caption">
      By singing up, you agree to the
      <span class="text-decoration-underline font-weight-medium"
        >Term of Service</span
      >
      and
      <span class="text-decoration-underline font-weight-medium"
        >Privacy Policy</span
      >
    </p>
  </v-form>
</template>

<script>
export default {
  name: "HelloWorld",

  data: () => ({}),
};
</script>
<style>
p {
  color: #f5f5f6;
}
.register-form {
  width: 600px;
  height: 660px;
  position: relative;
  border-top: 1px solid #86888f;
  border-radius: 12px;
  border-left: 1px solid #86888f;
}

.v-btn {
  text-transform: none;
}
.v-btn:hover {
  color: #cccccc;
}
.v-btn .v-ripple__container {
  color: #b3b3b3;
}
.gradient-text h3 {
  background: linear-gradient(270deg, #f5f5f6 0%, #95969d 100%);
  background-clip: text;
  -webkit-text-fill-color: transparent;
}
.v-btn--outlined {
  border-color: #62646d;
}
.theme--dark.v-input:hover {
  border-color: #cccccc;
}

.v-text-field--outlined:hover fieldset {
  border-color: #808080 !important;
  transition-property: color;
}

.v-text-field--outlined:hover fieldset,
.v-text-field--outlined:focus-within fieldset {
  color: #ffffff !important;
}
</style>
