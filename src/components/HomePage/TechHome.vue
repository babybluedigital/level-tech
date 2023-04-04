<template>
    
    <!-- Hero Section Starts -->
    
    <TechHomeHero />     
    
    <!-- Hero Section Ends -->
    
    <!-- Logo Section Starts -->
    
    <TechHomelogos />
    
    <!-- Logo Section Ends -->
    
    <!-- CTA Block Starts -->
    
    <TechHomeCtaBlock />
    
    <!-- CTA Block Ends -->
    
    <!-- Testimonial Starts Here -->
    
    <TechHomeTestimonial />
    
    <!-- Testimonial Ends Here -->
    
    <!-- Case Studies Start Here -->
    
    <TechHomeCaseStudies />
    
    <!-- Case Studies End Here -->
    
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
        TechHomeHero,
        TechHomeCtaBlock,
        TechHome4Block,
        TechHomeDemoBlock,
        TechHomeLearn,
        TechHomelogos,
        TechHomeReady,
        TechHomeTestimonial,
        TechHomeCaseStudies,
    }
}

</script>