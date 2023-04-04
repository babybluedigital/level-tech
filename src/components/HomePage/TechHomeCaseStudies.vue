<template>
    
    <!-- Learn Section Starts -->
    
    <section class="learn-section">
        
        <div>
            <h2>Want to learn more?</h2>
            <h6>Learn how LevelTech can deliver your results.</h6>
        </div>
        
        <div>
            
            <v-card class="mx-auto" max-width="400">
                <v-img class="align-end text-white" height="200" src="https://cdn.vuetifyjs.com/images/cards/docks.jpg" cover>
                    <v-card-title></v-card-title>
                </v-img>
                
                <v-card-subtitle class="pt-4">
                    Product Demo
                </v-card-subtitle>
                
                <v-card-text>
                    <div>See how LevelTech works with a short product demo.</div>
                </v-card-text>
                
                <v-card-actions>
                    <v-btn color="orange">
                        Book Now
                    </v-btn>
                </v-card-actions>
            </v-card>
            
            <v-card class="mx-auto" max-width="400">
                <v-img class="align-end text-white" height="200" src="https://cdn.vuetifyjs.com/images/cards/docks.jpg" cover>
                    <v-card-title></v-card-title>
                </v-img>
                
                <v-card-subtitle class="pt-4">
                    Case Studies
                </v-card-subtitle>
                
                <v-card-text>
                    <div>See how LevelTech has helps other sporting codes.</div>
                </v-card-text>
                
                <v-card-actions>
                    <v-btn color="orange">
                        Book Now
                    </v-btn>
                </v-card-actions>
            </v-card>
            
            <v-card class="mx-auto" max-width="400">
                <v-img class="align-end text-white" height="200" src="https://cdn.vuetifyjs.com/images/cards/docks.jpg" cover>
                    <v-card-title></v-card-title>
                </v-img>
                
                <v-card-subtitle class="pt-4">
                    Resources
                </v-card-subtitle>
                
                <v-card-text>
                    <div>Learn more with our dedicated resources.</div>
                </v-card-text>
                
                <v-card-actions>
                    <v-btn color="orange">
                        Book Now
                    </v-btn>
                </v-card-actions>
            </v-card>
            
        </div>
        
    </section>
    
    <!-- Learn Section Ends -->
    
</template>

<script>
import DunlopLogo from '@/assets/images/DunlopLogo.png';
import ESLogo from '@/assets/images/ESLogo.png';
import PSALogo from '@/assets/images/PSALogo.png';
import SportyLogo from '@/assets/images/SportyLogo.png';
import SquashSkillsLogo from '@/assets/images/SquashSkillsLogo.png';

export default {
    data() {
        return {
            logoItems: [
            { href: DunlopLogo },
            { href: ESLogo },
            { href: PSALogo },
            { href: SportyLogo },
            { href: SquashSkillsLogo },
            ],
        };
    },
};
</script>