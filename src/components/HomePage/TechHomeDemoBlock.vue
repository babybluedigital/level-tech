<style>

.demo_section {
    display: flex;
    flex-direction: column;
    gap: 60px;
}

.demo_button {
    background-color: transparent !important;
    border-color: transparent !important;
    font-weight: 700 !important;
    color: #000 !important;
    border-width: 0px !important;
}

.demo_button_group {
    display: flex;
    flex-direction: row;
    gap: 30px;
}

</style>

<template>
    
    <!-- Demo Block Section Starts Here -->
    
    <section class="demo_section">
        
        <div>
            
            <h1>Ready To Try LevelTech?</h1>
            
        </div>
        
        <div class="demo_button_group">
            
            <v-btn variant="tonal">Get Started</v-btn>
            <v-btn class="demo_button" append-icon="mdi-arrow-right" variant="outlined" scoped>Request Demo</v-btn>
            
        </div>
        
    </section>
    
    <!-- Demo Block Section Ends Here -->
    
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