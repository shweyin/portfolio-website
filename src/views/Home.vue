<template>
  <v-img src="@/assets/background.jpg">
    <v-row>
      <v-col cols="3">
        <v-timeline dense>            
          <v-hover v-slot:default="{hover}" close-delay="1000">
            <v-timeline-item fill-dot color="blue-grey" icon="mdi-account">
              <v-expand-transition>
                <v-card v-if="hover">
                  <v-card-title ><v-avatar class="mx-1"><v-img src="@/assets/profile.jpg"></v-img></v-avatar>Welcome to my Website!</v-card-title>
                  <v-card-text>This is currently a work in progress. I work on this website in my free time.</v-card-text>            
                </v-card>
              </v-expand-transition>              
            </v-timeline-item>
          </v-hover>
          <v-hover v-slot:default="{hover}" close-delay="1000">
            <v-timeline-item fill-dot color="blue-grey" icon="mdi-card-text-outline">
              <v-expand-transition>
                <v-card v-if="hover">
                  <v-card-text>My name is Shweyin. I'm taking an Honors Bachelors in Software Developing. This website is a hobby project that I'm working on to learn VueJS.</v-card-text>                  
                </v-card>
              </v-expand-transition>              
            </v-timeline-item>
          </v-hover>
          <v-hover v-slot:default="{hover}" close-delay="1000">
            <v-timeline-item fill-dot color="blue-grey" icon="mdi-script-text-outline">
              <v-expand-transition>
                <v-card v-if="hover">
                  <v-card-text>I'm currently searching for Co-op opportunities for Summer 2020 and Winter 2020! Here's a link to my <a href="./assets/Shweyin_Than_Resume.pdf" download>resume</a>.</v-card-text>
                  
                </v-card>
              </v-expand-transition>              
            </v-timeline-item>
          </v-hover>              
        </v-timeline>
      </v-col>
    </v-row>
    
  </v-img>  
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
</style>