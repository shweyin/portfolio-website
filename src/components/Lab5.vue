<template>
    <v-container>
        <v-card>
            <v-container>
                <v-row><v-card-title>Multimedia: Video</v-card-title></v-row>
                <v-row>
                    <v-col><v-card-text>I took a short video that I took a while ago and editted it to match the requirements of the assignment. I created a title page and end page in powerpoint and clipped the video so all 
                together the video would be a minute long. Then I clipped the background music as well and sped it up so that the section I wanted would fit just nicely into a minute long video. Finally
                I added the naration titles to match with the video and the music. This was all done in Open Shot. I exported the video in mp4 format and uploaded it to my website.</v-card-text></v-col>
                    <v-col>
                        <v-card-text>
                            <video width="700" height="400" controls>
                                <source src="@/assets/lab5BTH645.mp4" type="video/mp4">
                                Your browser does not support the video tag.
                            </video>
                        </v-card-text>
                    </v-col>
                </v-row>
            </v-container>
        </v-card>
    </v-container>
</template>

<script>
export default {
    
}
</script>