<style scoped>

.logo-section {
    display: flex;
    flex-direction: column;
    align-content: center;
    justify-content: space-between;
    align-items: center;
    gap: 45px;
    padding: 5% 2%;
    flex-wrap: wrap;
}

.logo-grid {
display: flex;
    flex-direction: row;
    gap: 25px;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
}

.v-card {
    display: flex;
    padding: 25px 30px;
    min-height: 120px;
    justify-content: center;
    align-items: center;
    border: 0px;
    border-radius: 20px;
    background-color: #f1f1f1;
    filter: grayscale(99%);
    transition: all 0.3s ease-out;
}

.v-card:hover {
    filter: grayscale(0%);
}

</style>

<template>
    
    <!-- Logo Section Starts -->
    
    <section class="logo-section">
        
        <div>
            
            <h3>Thousands of players get their rating with LevelTech software</h3>
            
        </div>
        
        <div class="logo-grid" scoped>
            <v-card v-for="(item, index) in logoItems" :key="index" variant="outlined" scoped>
                <v-img :width="175" aspect-ratio="4/3" :src="item.href"></v-img>
            </v-card>
        </div>
        
    </section>
    
    <!-- Logo Section Ends-->
    
</template>

<script>
import DunlopLogo from '@/assets/images/DunlopLogo.png';
import ESLogoRed from '@/assets/images/ESLogoRed.png';
import PSAColor from '@/assets/images/PSAColor.png';
import SportyLogo from '@/assets/images/SportyLogo.png';
import SquashSkillsLogo from '@/assets/images/SquashSkillsLogo.png';

export default {
    data() {
        return {
            logoItems: [
            { href: DunlopLogo },
            { href: ESLogoRed },
            { href: SportyLogo },
            { href: SquashSkillsLogo },
            { href: PSAColor },
            ],
        };
    },
};
</script>