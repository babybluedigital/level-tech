<style scoped>

section {
    display: flex;
    flex-direction: column;
    align-content: center;
    justify-content: center;
    align-items: center;
    gap: 30px;
    padding: 5% 8%;
}

.hero-section {
    min-height: 70vh;
}

.column-section {
    flex-direction: row;
}

.column-section div {
    flex-direction: column;
}

div {
    display: flex;
    gap: 20px;
}

h3 {
    text-align: center;
}

</style>

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
            <v-img :width="300" aspect-ratio="4/3" cover src="https://cdn.vuetifyjs.com/images/parallax/material.jpg"></v-img>
        </div>
        
        <div>
            
            <h2>Deploy your rating system globally</h2>
            <h6>Skip the painful setup and development. LevelTech is a global, production-ready system. Skip all the custom dev work and feed your results directly into your ratings.</h6>
            <v-btn variant="outlined">Button</v-btn>
            
        </div>
        
    </section>
    
    <!-- Column Section Starts -->
    
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