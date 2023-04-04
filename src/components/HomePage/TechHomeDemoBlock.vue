<template>
    
    <!-- Hero Section Starts -->
    
    <section class="hero-section">
        
        <div scoped>
            
            <h1>Bring It All Together</h1>
            
        </div>
        
        <div scoped>
            
            <h3>Power your sport with the LevelTech rating system.<br>Built with a powerful API, allowing you to reach a global audience.</h3>
            
        </div>
        
        <div scoped>
            
            <v-btn variant="tonal">
                Button
            </v-btn>
            
            <v-btn variant="outlined">
                Button
            </v-btn>
            
        </div>
        
    </section>
    
    <!-- Hero Section Ends -->
    
    <!-- Logo Section Starts -->
    
    <section>
        
        <div>
            
            <h3>Thousands of players get their rating with LevelTech software</h3>
            
        </div>
        
        <div>
            <v-card v-for="(item, index) in logoItems" :key="index" variant="outlined">
                <v-img :width="300" aspect-ratio="4/3" :src="item.href"></v-img>
            </v-card>
        </div>
        
    </section>
    
    <!-- Logo Section Ends-->
    
    <!-- Column Section Starts -->
    
    <section class="column-section">
        
        <div>
            <v-img :width="500" aspect-ratio="4/3" cover src="https://cdn.vuetifyjs.com/images/parallax/material.jpg"></v-img>
        </div>
        
        <div>
            
            <h2>Deploy your rating system globally</h2>
            <h6>Skip the painful setup and development. LevelTech is a global, production-ready system. Skip all the custom dev work and feed your results directly into your ratings.</h6>
            <v-btn variant="outlined">Button</v-btn>
            
        </div>
        
    </section>
    
    <!-- Column Section Starts -->
    
    <!-- Testimonial Section Starts -->
    
    <section class="testimonial-section">
        
        <h2>“Time savings is the most important thing for us. It’s been massive. I can record 150 steps in five minutes with Scribe.”</h2>
        <h6>Mark Williams, CEO England Squash</h6>
        <v-img :width="300" aspect-ratio="4/3" cover src="src\assets\images\ESLogo.png"></v-img>
        
    </section>
    
    <!-- Testimonial Section Endss -->
    
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
    
    <!-- Ready Section Starts Here -->
    
<section>

<div>

    <h2>Ready To Try LevelTech?</h2>

</div>

<div>

    <v-btn variant="outlined">Get Started</v-btn>
    <v-btn append-icon="mdi-arrow-right" variant="outlined">Request Demo</v-btn>

</div>

</section>

    <!-- Ready Section Ends Here -->
    
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