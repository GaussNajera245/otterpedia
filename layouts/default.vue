<template>
  <v-app >

    <v-content>
        <nuxt />
    </v-content>

    <v-app-bar fixed hide-on-scroll app height="88">
      <img src="/new-logo.png" href="http://www.nutriapedia.com/" style="height: 60px;">
      <v-spacer />
      <v-btn text x-large color="#F5F5F5">About</v-btn>
      <v-btn text x-large color="#F5F5F5">Contact</v-btn>
      <v-btn text x-large color="#F5F5F5">Tests</v-btn>
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
      title: 'Otterpedia'
    }
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
