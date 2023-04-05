<style>

.block_section {
    position: relative;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    align-content: center;
    gap: 90px;
}

.block_section div {
    flex: 1 1 50px;
}

.block_left {
    display: flex;
    flex-direction: column;
}

.block_left_sub {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 50px;
}   

.block_left_sub span {
    display: flex;
    flex-direction: column;
    flex: 1 1 200px;
}   

p {
    color: #757c8a;
}


#hero-collage-3 {
    position: absolute;
    left: 2%;
    top: 135px;
    width: 100px;
}


</style>

<template>
    
    <section class="block_section">
        
        <div class="block_left">
            
            <div>
                
                <span>
                    <h4>Launch</h4>
                </span>

                <img  id="hero-collage-3" class="hero-collage" src="../../assets/images/VerifiedPink.svg">
                
            </div>
            
            <div class="block_left_sub">

                <span>
                    <h6>Get it ready.</h6>
                    <p>Import all your users with our one-click import function.</p>
                </span>
                <span>
                    <h6>Deploy to mobile first.</h6>
                    <p>Our platform is built mobile ready and responds to all screen sizes.</p>
                </span>
                <span>
                    <h6>Test the water.</h6>
                    <p>Work in our test environment to develop the perfect rating system.</p>
                </span>
                <span>
                    <h6>Submit for release.</h6>
                    <p>Our instant publish feature allows you to go live in one deployment.</p>
                </span>
            </div>
            
        </div>
        
        <div>
            <v-img class="align-end text-white" height="600" src="src/assets/images/92104-real-time-coding.gif">
            </v-img>
        </div>
        
    </section>
    
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