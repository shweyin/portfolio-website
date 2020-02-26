<template>
    <nav>        
        <v-toolbar flat color="indigo">
            <v-app-bar-nav-icon class="white--text" @click="drawer = true"></v-app-bar-nav-icon>
            <v-toolbar-title class="text-uppercase white--text font-weight-bold">
                <span>Portfolio Website</span>
                <span class="overline"> Shweyin Than</span>
            </v-toolbar-title>
            <v-spacer></v-spacer>
            <v-btn depressed dark class="indigo" router to="/BTH645">BTH645</v-btn>
            <v-btn icon color="white" router to="/"><v-icon>mdi-home</v-icon></v-btn>
        </v-toolbar>
        <v-navigation-drawer app temporary v-model="drawer" class="indigo darken-4">
            <v-list class="indigo darken-2">
                <v-list-item >
                    <v-list-item-avatar centered>
                        <v-img src="@/assets/profile.jpg"></v-img>                        
                    </v-list-item-avatar>
                    <v-list-item-content>
                        <v-list-item-title class="white--text">Shweyin Than</v-list-item-title>
                        <v-list-item-subtitle class="white--text caption">Software Developer</v-list-item-subtitle>
                    </v-list-item-content>                    
                </v-list-item>                
            </v-list>
            <v-list dark>
                <v-list-item v-for="link in links" :key="link.text" router :to="link.route">
                    <v-icon>{{ link.icon }} </v-icon>
                    <v-list-item-content right> {{ link.text }}</v-list-item-content>
                </v-list-item>

            </v-list>

        
        </v-navigation-drawer>

        
    </nav>    
</template>


<script>
export default {
    data() {
        return {
            drawer: false,
            links: [
                {icon: 'mdi-home', text: 'Home', route: '/'},
                {icon: 'mdi-folder', text: 'My Projects', route: '/projects'},
                {icon: 'mdi-play-network', text: 'BTH645', route: '/BTH645'}
            ]
        }
    }
}
</script>