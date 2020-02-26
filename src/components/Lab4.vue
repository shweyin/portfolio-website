<template>
    <v-container>
        <v-card>
            <v-container>
                <v-row><v-card-title>Multimedia: Audio</v-card-title></v-row>
                <v-row>
                    <v-col>
                        <v-card>
                            <v-card-title>Ukulele Solo Wav</v-card-title>
                            <v-card-text>
                                <audio controls>
                                <source src="@/assets/UkuleleSolo.wav" type="audio/mpeg">
                                Your browser does not support the audio element.
                                </audio>
                            </v-card-text>                        
                        </v-card>
                    </v-col>
                    <v-col>
                        <v-card>
                            <v-card-title>Ukulele Solo Mp3</v-card-title>
                            <v-card-text>
                                <audio controls>
                                <source src="@/assets/UkuleleSolo.mp3" type="audio/mpeg">
                                Your browser does not support the audio element.
                                </audio>
                            </v-card-text>                        
                        </v-card>
                    </v-col>
                    <v-col>
                        <v-card>
                            <v-card-title>Edited Ukulele Solo Wav</v-card-title>
                            <v-card-text>
                                <audio controls>
                                <source src="@/assets/EditedUkuleleSolo.wav" type="audio/mpeg">
                                Your browser does not support the audio element.
                                </audio>
                            </v-card-text>                        
                        </v-card>
                    </v-col>             
                </v-row>
                <v-row>
                    <v-card-text>
                        <ol>
                            <li>WAV format is a raw audio format which means the sound will be as organic as possible as no losses happen from compression. Audacity supports export to wav formats very easily which is why I chose it.</li>
                            <li>My website uses controls for dealing with the audio. The audio won't play without the users discretion and thus will not be annoying or in the way.</li>
                            <li>MP3's are very good when quality is not a huge concern as they save a lot of space and will allow your pages to continue to load quickly.</li>
                            <li>I used 4 different techniques to edit my audio file: audio inversion, adjusting speed, fadeout, and adding a 'wahwah' effect.</li>
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