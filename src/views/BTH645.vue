<template>
    <div class="BTH645">
        <!-- <h1 class="grey--text">BTH645</h1> -->
        <v-container class="my-5">
            <v-layout row>
                <v-tabs grow dark background-color="blue" hide-slider>
                    <v-tab>Labs</v-tab>
                    <v-tab>Assignments</v-tab>
                    <v-tab>Student Oath</v-tab>

                    <v-tab-item>
                        <v-tabs grow>
                            <v-tab>Lab 1</v-tab>
                            <v-tab>Lab 2</v-tab>
                            <v-tab>Lab 3</v-tab>
                            <v-tab>Lab 4</v-tab>
                            <v-tab>Lab 5</v-tab>
                            <v-tab>Lab 6</v-tab>
                            <v-tab-item><Lab1/></v-tab-item>                            
                            <v-tab-item><Lab2/></v-tab-item>                            
                            <v-tab-item><Lab3/></v-tab-item>                            
                            <v-tab-item><Lab4/></v-tab-item>                            
                            <v-tab-item><Lab5/></v-tab-item>                            
                            <v-tab-item><Lab6/></v-tab-item>                            
                        </v-tabs>                        
                    </v-tab-item>
                    <v-tab-item>
                        <v-tabs grow>
                            <v-tab>Assignment 1</v-tab>
                            <v-tab>Assignment 2</v-tab>
                            <v-tab>Assignment 3</v-tab>
                            <v-tab-item><Assignment1/></v-tab-item>
                            <v-tab-item><Assignment2/></v-tab-item>
                            <v-tab-item>ETA March 30</v-tab-item>
                        </v-tabs>                        
                    </v-tab-item>
                    <v-tab-item>
                        <StudentOath/>
                    </v-tab-item>
                </v-tabs>
            </v-layout>                    
        </v-container>
        <v-footer absolute>This page was last modified on 4/05/2020, 9:44:19 PM</v-footer>    
    </div>
</template>

<script>
import Assignment1 from '@/components/Assignment1'
import Assignment2 from '@/components/Assignment2'
import Lab1 from '@/components/Lab1'
import Lab2 from '@/components/Lab2'
import Lab3 from '@/components/Lab3'
import Lab4 from '@/components/Lab4'
import Lab5 from '@/components/Lab5'
import Lab6 from '@/components/Lab6'
import StudentOath from '@/components/StudentOath'

export default {
    components: {
        Lab1,
        Lab2,
        Lab3,
        Lab4,
        Lab5,
        Lab6,
        Assignment1,
        Assignment2,
        StudentOath
    },
    data(){
        return{
            items: [

            ]
        }
    }
}
</script>

<style scoped>
</style>