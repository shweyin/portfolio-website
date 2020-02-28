<template>
    <v-container>      
        <v-card>
            <v-container>
                <v-row>
                    <v-card-title>Multimedia: Images</v-card-title>
                </v-row>
                <v-row wrap>
                    <v-col cols="12" sm="4">
                        <v-hover v-slot:default="{hover}">
                            <v-card>                            
                                <v-img src="@/assets/florida2020.jpg" aspect-ratio="1">
                                    <v-expand-transition>
                                        <div 
                                        v-if="hover" 
                                        class="d-flex transition-fast-in-fast-out white darken-2 v-card--reveal display-3"
                                        style="height: 100%">
                                            Florida 2020</div>
                                    </v-expand-transition>                                    
                                </v-img>                                                            
                            </v-card>
                        </v-hover>                        
                    </v-col>
                    <v-col cols="12" sm="4">
                        <v-hover v-slot:default="{hover}">
                            <v-card>                            
                                <v-img src="@/assets/florida2020edit.jpg" aspect-ratio="1">
                                    <v-expand-transition>
                                        <div 
                                        v-if="hover" 
                                        class="d-flex transition-fast-in-fast-out white darken-2 v-card--reveal display-3"
                                        style="height: 100%">
                                            Florida 2020 Edit</div>
                                    </v-expand-transition>                                    
                                </v-img>                                                            
                            </v-card>
                        </v-hover>
                    </v-col>
                    <v-col cols="12" sm="4">
                        <v-hover v-slot:default="{hover}">
                            <v-card>                            
                                <v-img src="@/assets/keyboard.jpg" aspect-ratio="1">
                                    <v-expand-transition>
                                        <div 
                                        v-if="hover" 
                                        class="d-flex transition-fast-in-fast-out white darken-2 v-card--reveal display-3"
                                        style="height: 100%">
                                            Keyboard Drawing</div>
                                    </v-expand-transition>                                    
                                </v-img>                                                            
                            </v-card>
                        </v-hover>
                    </v-col>
                </v-row>
                <v-row>
                    <v-card-text>
                     I like this assignment because it has a scalable difficulty depending on how good you want your website to look. I like that I have the option to make it look really nice when I have time, but if I'm really busy during that week, I don't have to worry too much about it. I enjoyed fiddling around with images in photoshop as well as it gave me the chance to experiment and have fun. 
                     <ol>
                         <li>I lightened the colors on this image a lot in order for the words written in the sand to show better. I also made the sky colors much whiter so that the photo appears to be in the day time rather than sunset. </li>
                         <li>The size has gotten a little larger, however both images are jpg and originally quite small. The resolution of the image has not been affected.</li>
                         <li>I used a reference photo and drew ontop of that, filling in areas with color. My goal was to capture the areas with color and focus on the shadow being a different color without using a huge color palette. I only used 6 colors throughout. </li>
                     </ol>
                 </v-card-text> 
                </v-row>
            </v-container>         
        </v-card>
    </v-container>
</template>

<script>
export default {
    
}
</script>

<style scoped>
    .v-card--reveal {
        align-items: center;
        justify-content: center;
        opacity: .5;
        position: absolute;
        width: 100%;
    }
</style>

