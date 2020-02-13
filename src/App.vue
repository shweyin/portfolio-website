<template>
  <v-app>
    <Navbar/>
    <v-content class="content ma-5">
      <router-view></router-view>
    </v-content>
    <v-footer>This page was last modified on 2/10/2020, 11:17:32 AM</v-footer>
  </v-app>
</template>

<script>
import Navbar from '@/components/Navbar'
export default {
  name: 'App',
  components: {
    Navbar,
  },
  data: () => ({
  }),
};
</script>