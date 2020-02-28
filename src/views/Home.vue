<template>
  <div class="home">
    <!-- <h1 class="grey--text">Home</h1> -->
    <v-container class="my-5">
      <v-row>
        <v-col cols="4">
          <v-alert type="info">Welcome to my website! This website is currently a work in progress. Here is it's timeline!</v-alert>
          <v-timeline>
            <v-timeline-item v-for="item in timeline" :key="item.title">
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
        <v-col>
          <h1>Ongoing Projects</h1>
          <v-simple-table>
            <thead>
              <tr>
                <th>Project Name</th>                
              </tr>
            </thead>
          </v-simple-table>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>

export default {
  name: 'Home',
  data() {
    return {
      timeline: [
        {title: 'Creation of Portfolio Website', date: '2/11/2020', content: 'The inception of this website, created to house my school assignments.'},
        {title: 'Added Previously Completed Labs', date: '2/11/2020', content: 'I had been using a pure html/css website to host a few labs before rebasing it to use Vue. All future labs and assignments are going to be uploaded to this website.'},
        {title: 'Completed Assignment 1', date: '2/22/2020', content: 'Completion of Assignment 1 for BTH645'},
        {title: 'Completed Lab 5', date: '2/22/2020', content: 'Completion of Lab 5 for BTH645'},
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