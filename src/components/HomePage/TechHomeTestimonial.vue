<style>

.testimonial-section {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 15px;
    background-color: #fbf9f4;
    padding: 5% 15%;
}

h2 {
    color: #231842;
}

.quote-title {
    padding-top: 20px;
    font-family: 'DM Sans', sans-serif;
    color: #23184299;
    font-size: 22px;
    line-height: 105.5%;
    font-weight: 500;
    letter-spacing: -0.3px;
}

.testimonial_image {
    width: 150px;
}

</style>

<template>
 
    <!-- Testimonial Section Starts -->
    
    <section class="testimonial-section">
        
        <h2>“The value we are able to give to our users cannot be measured, LevelTech has provided a service unmatched in the industry.”</h2>
        <h3 class="quote-title">Mark Williams, CEO England Squash</h3>
        <img class="testimonial_image" src="../../assets/images/ESLogoRed.png">
        
    </section>
    
    <!-- Testimonial Section Endss -->
    
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