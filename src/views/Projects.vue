<template>
  <div class="projects ma-5">
    <h1 class="grey--text">My Projects</h1>
    <v-container class="my-5">
      <v-simple-table>
            <thead>
              <tr>
                <th>Name</th>
                <th>Start Date</th>
                <th>End Date</th>
                <th>Status</th>
              </tr>
            </thead>
            <tbody>
              <tr v-for="item in projects" :key="item.name">
                <td>{{item.name}}</td>
                <td>{{item.start}}</td>
                <td>{{item.end}}</td>
                <td>{{item.status ? "Ongoing" : "Finished"}}</td>
              </tr>
            </tbody>
          </v-simple-table>
    </v-container>
  </div>
</template>

<script>
export default {
  data(){
    return {
      projects: [
        {name: "Portfolio Website", link: "/", start: "2/27/2020", end: "", status: true},
        {name: "Add Database", link: "/", start: "2/27/2020", end: "", status: true},
        {name: "Add Past School Projects", link: "/", start: "2/27/2020", end: "", status: true},
        {name: "Add API", link: "/", start: "2/27/2020", end: "", status: true},
        {name: "Link to Capstone Project", link: "/", start: "2/27/2020", end: "", status: true},
      ]
    }
  }
}
</script>
