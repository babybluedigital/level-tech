<style scoped>

.learn-section {
    display: flex;
    flex-direction: column;
    gap: 40px;
    align-items: center;
}

.card_div {
    display: flex;
    flex-direction: row;
    gap: 30px;
    flex-wrap: wrap;
}

h3 {
    font-weight: 400;
    text-align: center;
    color: #757c8a;
}

.v-card {
    border-radius: 10px;
    flex: 1 1 250px;
    box-shadow: none;
    transition: all 0.3s ease-in-out;
}

.v-card:hover {
    box-shadow: 10px 20px 60px 0px rgba(0,0,0,0.1);
}

.card_details {
    display: flex;
    flex-direction: column;
} 

.v-btn--variant-plain {
    color: #000;
    text-transform: capitalize;
    font-weight: 500;
    font-size: 18px;
    font-family: Pacaembu,sans-serif;
    transition: all 0.2s ease-in-out;
}

.v-btn--variant-plain:hover {
    color: #4EE7C0;
}

.v-card .v-card-subtitle {
    font-size: 16px;
    font-family: Pacaembu,sans-serif;
}

.v-card .v-card-text {
    font-size: 17px;
    line-height: 1.5;
    font-weight: 500;
    font-family: Pacaembu,sans-serif;
}

</style>

<template>
    
    <!-- Learn Section Starts -->
    
    <section class="learn-section">
        
        <div>
            <h1>Want to learn more?</h1>
            <h3>Learn how LevelTech can deliver your results.</h3>
        </div>
        
        <div class="card_div" scoped>
            
            <v-card class="mx-auto" max-width="400">
                <v-img class="align-end text-white" height="200" src="src/assets/images/PaulGlaze.jpg" cover>
                    <v-card-title></v-card-title>
                </v-img>
                <div class="card_details">
                    <v-card-subtitle class="pt-4">
                        Product Demo
                    </v-card-subtitle>
                    
                    <v-card-text>
                        <div>See how LevelTech integrates into your system with our short product demo.</div>
                    </v-card-text>
                    
                    <v-card-actions>
                        <v-btn variant="plain">
                            Book Now
                        </v-btn>
                    </v-card-actions>
                </div>
            </v-card>
            
            <v-card class="mx-auto" max-width="400">
                <v-img class="align-end text-white" height="200" src="src/assets/images/MayaFriends.png" cover>
                    <v-card-title></v-card-title>
                </v-img>
                <div class="card_details">
                <v-card-subtitle class="pt-4">
                    Case Studies
                </v-card-subtitle>
                
                <v-card-text>
                    <div>See how LevelTech has supported a range of global sporting codes.</div>
                </v-card-text>
                
                <v-card-actions>
                    <v-btn variant="plain">
                        Read Now
                    </v-btn>
                </v-card-actions>
                </div>
            </v-card>
            
            <v-card class="mx-auto" max-width="400">
                <v-img class="align-end text-white" height="200" src="src/assets/images/PaddleBlue.png" cover>
                    <v-card-title></v-card-title>
                </v-img>
                <div class="card_details">
                <v-card-subtitle class="pt-4">
                    Resources
                </v-card-subtitle>
                
                <v-card-text>
                    <div>Find out more about what's possible with our dedicated LevelTech developer resources.</div>
                </v-card-text>
                
                <v-card-actions>
                    <v-btn variant="plain">
                        Learn Now
                    </v-btn>
                </v-card-actions>
                </div>
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