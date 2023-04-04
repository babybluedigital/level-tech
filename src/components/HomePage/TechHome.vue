<template>
    
    <!-- Hero Section Starts -->
    
    <div class="hero-section">
        <TechHomeHero />     
    </div>
    
    <!-- Hero Section Ends -->
    
    
    
    <!-- Logo Section Starts -->
    
    <div class="hero-section">
        <TechHomelogos />     
    </div>
    
    <!-- Logo Section Ends-->
    
    
    <!-- Column Section Starts -->
    
    <div class="hero-section">
        <TechHomeCaseStudies />     
    </div>
    
    <!-- Column Section Starts -->
    
    <!-- Column Section Starts -->
    
    <div class="hero-section">
        <TechHome4Block />     
    </div>
    
    <!-- Column Section Starts -->
    
    
    
    
    <!-- Testimonial Section Starts -->
    
    <div class="hero-section">
        <TechHomeTestimonial />     
    </div>
    
    <!-- Testimonial Section Endss -->
    
    
    
    <!-- Learn Section Starts -->
    
    <div class="hero-section">
        <TechHomeLearn />     
    </div>
    
    <!-- Learn Section Ends -->
    
    
    
    <!-- Ready Section Starts Here -->
    
    <div class="hero-section">
        <TechHomeReady />     
    </div>
    
    <!-- Ready Section Ends Here -->
    
</template>

<script>
import TechHomeHero from '../HomePage/TechHomeHero.vue';
import TechHomeCtaBlock from '../HomePage/TechHomeCtaBlock.vue';
import TechHome4Block from '../HomePage/TechHome4Block.vue';
import TechHomeDemoBlock from '../HomePage/TechHomeDemoBlock.vue';
import TechHomeLearn from '../HomePage/TechHomeLearn.vue';
import TechHomelogos from '../HomePage/TechHomeLogos.vue';
import TechHomeReady from '../HomePage/TechHomeReady.vue';
import TechHomeTestimonial from '../HomePage/TechHomeTestimonial.vue';
import TechHomeCaseStudies from '../HomePage/TechHomeCaseStudies.vue';

export default {
    components: {
        TechHomeHero
        TechHomeCtaBlock
        TechHome4Block
        TechHomeDemoBlock
        TechHomeLearn
        TechHomelogos
        TechHomeReady
        TechHomeTestimonial
        TechHomeCaseStudies
    }
}

</script>