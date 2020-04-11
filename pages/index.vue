<template>
  <v-layout column justify-center align-center>
    <v-carousel
      cycle
      height="470px"
      hide-delimiter-background
      :show-arrows="false"
      delimiter-icon="mdi-minus"
    >
      <v-carousel-item v-for="(slide,i) in slides" :key="i">
        <v-row class="fill-height" align="center" justify="center">
          <v-img :src="slide" />
        </v-row>
      </v-carousel-item>
    </v-carousel>

    <section id="apply-all">
      <h2>Learn More about Otters !!!</h2>
    </section>

    <section id="tests">
      <v-col style="padding-top: 39px;" class="fill-height" align="center" justify="center">
        <v-flex>
          <h1 style="font-size: 33px;">
            TESTS:
          </h1>
          <h3>You can get to know more with our various test about otter life like:</h3>
        </v-flex>

        <v-layout row justify-space-around>
          <v-flex v-for="(card,i) in cards1" :key="i" xs5>
            <br>
            <v-card style="padding-top: 12px;max-width: 470px;">
              <span>
                <v-icon>{{ card.fav }}</v-icon>
              </span>
              <span>
                <v-card-text>{{ card.title }}</v-card-text>
              </span>
            </v-card>
          </v-flex>
        </v-layout>
      </v-col>
    </section>

    <v-img id="about" src="/otter-hand2.jpg">
      <v-layout row justify-space-around style="height:100%">
        <v-flex class="translucid">
          <v-flex>
            <v-card-text>
              <h1 style="font-size: 33px;">
                ABOUT US:
              </h1>
            </v-card-text>
            <v-card-text>
              <h3>There has been plenty of research relating to Otters over the years. As a result we do know quite a bit about these animals. We do know that they have been around for millions of years. They were once creatures that were only on land but then they adapted to a life that allows them to be in the water as well. We know that they are meat eaters and that they aren’t very picky when it comes to the prey they find.</h3>
            </v-card-text>
            <v-card-text>
              <h3>There has been plenty of research relating to Otters over the years. As a result we do know quite a bit about these animals. We do know that they have been around for millions of years. They were once creatures that were only on land but then they adapted to a life that allows them to be in the water as well. We know that they are meat eaters and that they aren’t very picky when it comes to the prey they find.</h3>
            </v-card-text>
            <v-card-text>
              <h3>There has been plenty of research relating to Otters over the years. As a result we do know quite a bit about these animals. We do know that they have been around for millions of years. They were once creatures that were only on land but then they adapted to a life that allows them to be in the water as well. We know that they are meat eaters and that they aren’t very picky when it comes to the prey they find.</h3>
            </v-card-text>
            <v-card-text>
              <h3>There has been plenty of research relating to Otters over the years. As a result we do know quite a bit about these animals. We do know that they have been around for millions of years. They were once creatures that were only on land but then they adapted to a life that allows them to be in the water as well. We know that they are meat eaters and that they aren’t very picky when it comes to the prey they find.</h3>
            </v-card-text>
          </v-flex>
        </v-flex>
      </v-layout>
    </v-img>

    <v-container id="contact">
      <v-flex>
        <formate />
      </v-flex>
    </v-container>
  </v-layout>
</template>

<script>
import formate from '~/components/formate.vue'

export default {
  components: {
    formate
  },
  data () {
    return {
      slides: ['/sup.jpg', '/otters-group.jpg', '/sea-otter-wild.jpg'],
      cards1: [
        { title: 'Etymology', fav: 'launch' },
        { title: 'Feeding', fav: 'fastfood' },
        { title: 'Life Cycle', fav: 'favorite' },
        { title: 'Description', fav: 'list' },
        { title: 'Species', fav: 'opacity' },
        { title: 'Habitat', fav: 'home' },
        { title: 'Terminology', fav: 'fingerprint' },
        { title: 'Fun facts', fav: 'grade' }
      ]
    }
  }
}
</script>

<style>
#apply-all {
  margin-top: 25px;
  margin-bottom: 25px;
}

#about {
  margin-top: 25px;
  margin-bottom: 25px;
}

#tests {
  height: 630px;
  margin-top: 25px;
  margin-bottom: 25px;
  width: 100%;
  background-color: #4e453c;
}

h2 {
  font-style: oblique;
  font-size: xxx-large;
  color: #f5f5f5;
  text-align: center;
}

.translucid {
  background-color: #fbc15d;
  opacity: 0.5;
  padding-left: 12px;
  padding-right: 12px;
  padding-top: 44px;
}

.my-span {
  /* background-color: blue; */
  color: black;
  font-weight: bold;
  margin-right: 0;
  float: right;
}
</style>
