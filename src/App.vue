<template>
  <v-app>
    <v-app-bar
      app
      color="dark"
      dark
      class="drag-area"
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <HelloWorld/>
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld'

export default {
  name: 'App',

  components: {
    HelloWorld
  },

  data: () => ({
    //
  })
}
</script>

<style>
  /* CSS */

:not(input):not(textarea),
:not(input):not(textarea)::after,
:not(input):not(textarea)::before {
    -webkit-user-select: none;
    user-select: none;
    cursor: default;
}
input, button, textarea, :focus {
    outline: none;
}

  /* General Restyling */
.text-shadow-sm,
.text-shadow-small {
   text-shadow: 2px 2px 2px rgba(80, 80, 80, 0.1)
}
.text-shadow,
.text-shadow-md,
.text-shadow-medium {
   text-shadow: 4px 4px 4px rgba(80, 80, 80, 0.1)
}
.text-white {
  color: #fff;
}
.text-grey,
.text-gray {
  color: #6c757d;
}

.bg-off-black {
  background-color: #222 !important;
}

.bg-wilbur {
  background-color: rgb(62, 199, 62) !important;
}
.bg-light-pink {
  background-color: rgb(255,230,230) !important;
}
.bg-light-blue {
  background-color: rgb(230,230,255) !important;
}

.vh-75 {
  height: 75vh;
}
.vh-50 {
  height: 50vh;
}
.vh-25 {
  height: 25vh;
}
.vh-10 {
  height: 10vh;
}

.inverted {
filter: invert(100%);
}

.text-center {
  text-align: center;
}

.fit-fill {
  object-fit: fill;
}
.fit-contain {
  object-fit: contain;
}
.fit-cover {
  object-fit: cover;
}
.fit-scale-down {
  object-fit: scale-down;
}
.fit-none {
  object-fit: none;
}
::placeholder {
  color: #f8f9fa !important;
  opacity: 1 !important;
}
input:active,
input:focus,
button:active,
button:focus {
  box-shadow: none !important;
}

a{
  text-decoration: none !important;
}

.drag-area {
  -webkit-app-region: drag
}
.no-drag {
  -webkit-app-region: no-drag;
  cursor: auto;
}
.grab {
  cursor: pointer;
}

/* Transition Styling */
.fade-enter-active, .fade-leave-active {
  transition: opacity .5s;
}
.fade-enter, .fade-leave-to /* .fade-leave-active below version 2.1.8 */ {
  opacity: 0;
}

.slide-up-enter-active, .slide-up-leave-active {
  transition: transform 0.75s;
}
.slide-up-enter, .slide-up-leave-to {
  transform: translateY(-100vh);
}

.custom-enter,
.custom-enter-active {
  transition-duration: 1s;
  transition-property: opacity transform;
  transition-timing-function: ease;
  opacity: 0;
  transform: translateY(-2vh);
}
.custom-leave,
.custom-leave-active {
  transition-duration: 1s;
  transition-property: opacity transform;
  transition-timing-function: ease;
  opacity: 0;
  transform: translateY(2vh);
}

/* hovers */
.hover-light {
  background-color: #343a40 !important;
  color: #f8f9fa !important;
}
.hover-light:hover {
  background-color: #f8f9fa !important;
  color: #343a40 !important;
}
.hover-invert:hover {
filter: invert(100%);
}

</style>
