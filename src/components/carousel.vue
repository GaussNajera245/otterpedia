<template>
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
</template>

<script>
export default {
  name: "carrousel",
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
