<template>
  <v-app>
    <link
      href="https://fonts.googleapis.com/css?family=Roboto:100,300,400,500,700,900|Material+Icons"
      rel="stylesheet"
    >
    <v-content>
      <nuxt />
    </v-content>

    <v-app-bar fixed hide-on-scroll app height="88">
      <img
        src="/new-logo.png"
        style="height: 60px;"
        @click="$vuetify.goTo('http://www.nutriapedia.com/', options)"
      >
      <v-spacer />
      <v-btn text x-large color="#F5F5F5" @click="$vuetify.goTo('#about', options)">
        About
      </v-btn>
      <v-btn text x-large color="#F5F5F5" @click="$vuetify.goTo('#contact', options)">
        Contact
      </v-btn>
      <v-btn text x-large color="#F5F5F5" @click="$vuetify.goTo('#tests', options)">
        Tests
      </v-btn>
    </v-app-bar>

    <v-footer>
      <span>&copy; 2019 Web Dev</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      title: 'Otterpedia',
      duration: 1000,
      offset: -60,
      easing: 'easeInOutCubic'
    }
  },
  computed: {
    options () {
      return {
        duration: this.duration,
        offset: this.offset,
        easing: this.easing
      }
    }
  },
  head () {
    return {
      title: this.title,
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        { hid: 'otterpedia', name: 'Otterpedia', content: 'Learn More about Otters !!!' }
      ]
    }
  }
}
</script>

<style>
.container {
  padding-left: 0px;
  padding-right: 0px;
  padding-top: 0px;
}
</style>
