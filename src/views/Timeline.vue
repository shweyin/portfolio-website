<template>
    <v-container class="my-5">
      <v-row no-gutters>
        <v-col>
          <v-alert type="info">Welcome to my website! This website is currently a work in progress. Here is it's timeline!</v-alert>
          <v-timeline>
            <v-timeline-item v-for="item in timeline" :key="item.title">
                <template v-slot:opposite>
                    <span>{{item.date}}</span>
                </template>
                <v-card min-width="240" elevation="8">              
                    <v-card-title class="blue">
                        <h2 class="white--text font-weight-light">{{ item.title }}</h2>
                    </v-card-title>
                    <v-container>
                    <v-card-text>{{item.content}}</v-card-text>
                    </v-container>
              </v-card>
            </v-timeline-item>
          </v-timeline>
        </v-col>
      </v-row>
    </v-container>
</template>

<script>

export default {
  name: 'Timeline',
  data() {
    return {
      timeline: [
        {title: 'Create Portfolio Website', date: '2/11/2020', content: 'Port from old html/css website to VueJS'},
        {title: 'Complete Assignments', date: '2/22/2020', content: 'Complete Assignment 1 and Lab5 for BTH645'},
        {title: 'Deloy to Heroku', date: '2/24/2020', content: 'Setup automatic deployment from Github Repo to Heroku'},
        {title: 'Update Style', date: '3/1/2020', content: 'Update Home Page, change NavBar theme'},
        // {title: '', date: '', content: ''},
      ]
    }
  },
  components: {
  }
}
</script>

<style scoped>
</style>