<template>
  <v-app >

    <v-content>
        <nuxt />
    </v-content>

    <v-app-bar fixed hide-on-scroll app height="88">
      <img src="/new-logo.png"  @click="$vuetify.goTo('http://www.nutriapedia.com/', options)" style="height: 60px;">
      <v-spacer />
      <v-btn text x-large color="#F5F5F5" @click="$vuetify.goTo('#about', options)">About</v-btn>
      <v-btn text x-large color="#F5F5F5" @click="$vuetify.goTo('#contact', options)" >Contact</v-btn>
      <v-btn text x-large color="#F5F5F5" @click="$vuetify.goTo('#tests', options)">Tests</v-btn>
    </v-app-bar>

    <v-footer >
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
          easing: this.easing,
        }
      },
}
}
</script>


<style>

  .container{
    padding-left: 0px;
    padding-right: 0px;
    padding-top: 0px;
  }

</style>
