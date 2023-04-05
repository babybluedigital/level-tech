<style scoped>

.hero-section {
    min-height: 100vh;
}

.hero-section-center {
    display: flex;
    flex-direction: column;
    align-content: center;
    justify-content: center;
    align-items: center;
    gap: 25px;
    flex-grow: 1;
}

.hero-section-left {
    display: flex;
    flex-direction: column;
    flex-basis: 18%;
}

.hero-section-right {
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    flex-basis: 18%;
}

.hero-background-block {
    max-width: 115px;
    z-index: 0;
}

div .hero-background-block:first-child {
    position: absolute;
    bottom: 14%;
    left: 31%;
}

div .hero-background-block:nth-child(2) {
    position: absolute;
    top: 18%;
    right: 25%;
}

div .hero-background-block:nth-child(3) {
    position: absolute;
    bottom: 9%;
    left: 65%
}

div .hero-background-block:nth-child(4) {
    position: absolute;
    top: 20%;
    left: 17%;
}

div .hero-background-block:nth-child(5) {
    position: absolute;
    top: 13%;
    left: 35%;
}


div {
    display: flex;
    gap: 25px;
}

h1, h3 {
    text-align: center; 
}

.v-img {
    max-width: 100px;
}

.v-btn--variant-tonal {
    background-color: #4EE7C0;
    border-color: #4EE7C0;
    font-size: 18px;
    font-family: Pacaembu,sans-serif;
    font-weight: 700;
    color: #fff;
    text-transform: capitalize;
}

.v-btn--variant-outlined {
    background-color: transparent;
    border-color: #4EE7C0;
    font-weight: 700;
    color: #4EE7C0;
    border-width: 3px;
    
}

img {
    transition: all 0.3s ease-out;
}

.hero-collage {
    max-width: 450px;
    z-index: 1;
    transition: all 0.3s ease-out;
}

#hero-collage-1 {
    bottom: 10%;
    position: absolute;
    left: -7%;
}

#hero-collage-1:hover {
    transform: scale(1.1) translateX(20px);
    cursor: grab;
}

#hero-collage-2 {
    bottom: 15%;
    position: absolute;
    right: -7%;
}

#hero-collage-2:hover {
    transform: scale(1.1) translateX(-20px);
    cursor: grab;
}

</style>

<template> 
    
    <!-- Hero Section Starts -->
    
    <section class="hero-section">
        
        <div class="hero-section-left">
            
            <img  id="hero-collage-1" class="hero-collage" src="../../assets/images/HeroCollage1.png">
            
        </div>
        
        
        <div class="hero-section-center" scoped>
            
            <div scoped>
                
                <h1>Bring It All Together</h1>
                
            </div>
            
            <div scoped>
                
                <h3>Bringing Data-Driven Accuracy to Sports Ratings.<br>Built with a powerful API, allowing you to reach a global audience.</h3>
                
            </div>
            
            <div scoped>
                
                <v-btn variant="tonal">
                    Learn More
                </v-btn>
                
                <v-btn variant="outlined">
                    Request A Demo
                </v-btn>
                
            </div>
            <div>
                
                <img class="hero-background-block" src="../../assets/images/GreyBlock.png">
                <img class="hero-background-block" src="../../assets/images/GreyBlock.png">
                <img class="hero-background-block" src="../../assets/images/GreyBlock.png">
                <img class="hero-background-block" src="../../assets/images/GreyBlock.png">
                <img class="hero-background-block" src="../../assets/images/GreyBlock.png">
                
            </div>
            
            
        </div>
        
        
        <div class="hero-section-right">
            
            <img id="hero-collage-2" class="hero-collage" src="../../assets/images/HeroCollage2.png">
            
        </div>
        
    </section>
    
    <!-- Hero Section Ends -->
    
</template>

<script>

import HeroCollage1 from '@/assets/images/HeroCollage1.png';
import HeroCollage2 from '@/assets/images/HeroCollage2.png';

export default {
    data() {
        return {
            heroItems: [
            { href: HeroCollage1 },
            { href: HeroCollage2 },
            ],
        };
    },
};

</script>