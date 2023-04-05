<template>
    
    <!-- Hero Section Starts -->
    <TechHomeHero />     
    
    <!-- Logo Section Starts -->
    <TechHomelogos />
    
    <!-- CTA Block Starts -->
    <TechHomeCtaBlock />
    
    <!-- 4 Block Section -->
    <TechHome4Block />
    
    <!-- Testimonial Starts Here -->
    <TechHomeTestimonial />
    
    <!-- Case Studies Start Here -->
    <TechHomeCaseStudies />
    
    <!-- Demo Block -->
    <TechHomeDemoBlock />
    
</template>

<script>
import TechHomeHero from '../HomePage/TechHomeHero.vue';
import TechHomeCtaBlock from '../HomePage/TechHomeCtaBlock.vue';
import TechHome4Block from '../HomePage/TechHome4Block.vue';
import TechHomeDemoBlock from '../HomePage/TechHomeDemoBlock.vue';
import TechHomeLearn from '../HomePage/TechHomeLearn.vue';
import TechHomelogos from '../HomePage/TechHomeLogos.vue';
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
        TechHomeTestimonial,
        TechHomeCaseStudies,
    }
}

</script>