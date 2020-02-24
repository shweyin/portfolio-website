<template>
    <v-container>
        <v-card>
            <v-card-title>Multimedia: Audio</v-card-title>
            <v-card-text>
                <div>Ukulele Solo Wav</div>
                <audio controls>
                <source src="@/assets/UkuleleSolo.wav" type="audio/mpeg">
                Your browser does not support the audio element.
                </audio> 
                <div>Ukulele Solo Mp3</div>
                <audio controls>
                <source src="@/assets/UkuleleSolo.mp3" type="audio/mpeg">
                Your browser does not support the audio element.
                </audio>
                <div>Edited Ukulele Solo Wav</div>
                <audio controls>
                <source src="@/assets/EditedUkuleleSolo.wav" type="audio/mpeg">
                Your browser does not support the audio element.
                </audio>
                <ol>
                    <li>WAV format is a raw audio format which means the sound will be as organic as possible as no losses happen from compression. Audacity supports export to wav formats very easily which is why I chose it.</li>
                    <li>My website uses controls for dealing with the audio. The audio won't play without the users discretion and thus will not be annoying or in the way.</li>
                    <li>MP3's are very good when quality is not a huge concern as they save a lot of space and will allow your pages to continue to load quickly.</li>
                    <li>I used 4 different techniques to edit my audio file: audio inversion, adjusting speed, fadeout, and adding a 'wahwah' effect.</li>
                </ol>
            </v-card-text>
        </v-card>
    </v-container>
</template>

<script>
export default {
    
}
</script>