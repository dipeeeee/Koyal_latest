<template>
  <v-app id="inspire">
    <v-app-bar extended>
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
      <v-app-bar-title>Nature Gallery</v-app-bar-title>
      <v-spacer></v-spacer>
      <v-btn icon="mdi-dots-vertical"></v-btn>
    </v-app-bar>

    <v-main>
      <v-container>
        <v-row>
          <!-- Loop through images array -->
          <v-col
            v-for="(image, index) in images"
            :key="index"
            cols="4"
          >
            <v-card height="200" >
              <!-- Use dynamic image source -->
              <v-img
                :src="image"
                alt="Nature Image"
                aspect-ratio="1.78"
              ></v-img>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      // Array of different image URLs
      images: [
        "https://images.pexels.com/photos/381739/pexels-photo-381739.jpeg?auto=compress&cs=tinysrgb&w=600",
        "https://images.pexels.com/photos/326055/pexels-photo-326055.jpeg?auto=compress&cs=tinysrgb&w=600",
        "",
        "https://source.unsplash.com/500x500/?nature,beach",
        "https://source.unsplash.com/500x500/?nature,lake",
        "https://source.unsplash.com/500x500/?nature,desert",
        "https://source.unsplash.com/500x500/?nature,animals",
        "https://source.unsplash.com/500x500/?nature,flowers",
        "https://source.unsplash.com/500x500/?nature,sunrise",
        "https://source.unsplash.com/500x500/?nature,sunset",
        "https://source.unsplash.com/500x500/?nature,forest,mist",
        "https://source.unsplash.com/500x500/?nature,rivers",
        "https://source.unsplash.com/500x500/?nature,clouds",
        "https://source.unsplash.com/500x500/?nature,countryside",
        "https://source.unsplash.com/500x500/?nature,plants",
        "https://source.unsplash.com/500x500/?nature,spring",
        "https://source.unsplash.com/500x500/?nature,autumn",
        "https://source.unsplash.com/500x500/?nature,snow",
        "https://source.unsplash.com/500x500/?nature,rain",
        "https://source.unsplash.com/500x500/?nature,night",
        "https://source.unsplash.com/500x500/?nature,storm",
        "https://source.unsplash.com/500x500/?nature,cliff",
        "https://source.unsplash.com/500x500/?nature,rock",
        "https://source.unsplash.com/500x500/?nature,hills"
      ]
    };
  }
};
</script>

<style scoped>
/* You can add any custom styles here */
</style>
