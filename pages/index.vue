<template>
  <v-layout column justify-center align-center >
     <v-carousel
        cycle
        heigh="500px"
        hide-delimiter-background
        :show-arrows="false"
        delimiter-icon="mdi-minus"
      >
        <v-carousel-item  
          v-for="(slide,i) in slides"  
          :key='i' >
            <v-row  
              class="fill-height" 
              align="center" 
              justify="center" >
                <v-img :src="slide"></v-img>
            </v-row>
        </v-carousel-item>
      </v-carousel>
    
      
    <v-col class="fill-height" align="center" justify="center">
      <v-flex>
        <h2 > Learn More about Otters !!! </h2>
      </v-flex>
       
      <v-layout row justify-space-between>

            <v-flex>

              
              <v-card class="justify-center" > Etymology</v-card>
              <v-card class="justify-center" > Life Cycle</v-card>
              <v-card class="justify-center" > Description</v-card>
              
            </v-flex>

            <v-flex>

              
              <v-card class="justify-center" > Feeding</v-card>
              <v-card class="justify-center" > Terminology</v-card>
              <v-card class="justify-center" > Species</v-card>
              
            </v-flex>

          </v-layout>
    </v-col>  



    




        
        
        



    <v-img src="/otter-hand.jpg"></v-img>
    <v-img src="/otter-hand.jpg" width="100%" position="absolute"  ></v-img>
    <v-img src="/otter-hand.jpg" width="100%" position="absolute"  ></v-img>


  
  </v-layout>
</template>

<script>
// import Logo from '~/components/Logo.vue'
// import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  // components: {
  //   Logo,
  //   VuetifyLogo
  // },   
  data () {
      return {
        slides: [
          "/sup.jpg",
          "/otters-group.jpg",
          "/sea-otter-wild.jpg",
        ],
      }
  }
}
</script>


<style>
 #text-section-gn{
    margin-top: 25px;
    margin-bottom: 25px;
    padding-top: 25px; 
 }
</style>
