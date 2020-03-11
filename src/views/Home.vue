<template>
  <div class="background">
  <!-- <v-img src="@/assets/background.jpg" class="background-image" > -->
    <v-row no-gutters>
      <v-col cols="11" md="6" lg="3">
        <v-timeline dense>            
          <v-hover v-slot:default="{hover}" close-delay="5000">
            <v-timeline-item fill-dot color="blue-grey" icon="mdi-account">
              <v-expand-transition>
                <v-card v-if="hover">
                  <v-card-title ><v-avatar class="mx-1"><v-img src="@/assets/profile.jpg"></v-img></v-avatar>Welcome to my Website!</v-card-title>
                  <v-card-text>At the moment, this website is hosting my assignments from BTH645 and is my passion project. I will be building up this website to use as my portfolio.</v-card-text>
                  <v-card-actions class="justify-center">
                    <v-btn icon><a href="https://www.linkedin.com/in/shweyin-than-656153130/" target="_blank"><v-icon>mdi-linkedin</v-icon></a></v-btn>
                    <v-btn icon><a href="https://github.com/shweyin" target="_blank"><v-icon>mdi-git</v-icon></a></v-btn>
                  </v-card-actions>
                </v-card>
              </v-expand-transition>              
            </v-timeline-item>
          </v-hover>
          <v-hover v-slot:default="{hover}" close-delay="5000">
            <v-timeline-item fill-dot color="blue-grey" icon="mdi-card-text-outline">
              <v-expand-transition>
                <v-card v-if="hover">
                  <v-card-text>My name is Shweyin. I'm taking an Honors Bachelors in Software Developing. This website is a hobby project that I'm working on to learn VueJS.</v-card-text>                  
                </v-card>
              </v-expand-transition>              
            </v-timeline-item>
          </v-hover>
          <v-hover v-slot:default="{hover}" close-delay="5000">
            <v-timeline-item fill-dot color="blue-grey" icon="mdi-script-text-outline">
              <v-expand-transition>
                <v-card v-if="hover">
                  <v-card-text>I'm currently searching for Co-op opportunities for Summer 2020 and Winter 2020! Here's a link to my <a href="https://docs.google.com/document/d/1cCyRzBIn2SmYIzRKg1cvlnWPZ8LV2PJtDibnQyvRWAM/edit?usp=sharing" download>resume</a>.</v-card-text>
                  
                </v-card>
              </v-expand-transition>              
            </v-timeline-item>
          </v-hover>              
        </v-timeline>
      </v-col>
    </v-row>
  </div>
    
  <!-- </v-img>   -->
</template>

<script>

export default {
  name: 'Home',
  data() {
    return {
    }
  },
  components: {
  }
}
</script>

<style scoped>
.background {
  background-image: url("../assets/background.jpg");
  height: 100%;
  width: 100%;
  background-size: cover;
}
</style>