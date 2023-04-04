<style>

.column-section {
    display: flex;
    flex-direction: row;
    gap: 130px;
}

.column-section div {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: start;
    gap: 40px;
}

v-div {
    flex: 1;
}

.cta-img {
    width: auto !important;
    border-radius: 10px;
    box-shadow: -25px 20px 2px 0px hsl(165,76%,65%, 0.5);
}

.v-btn--variant-tonal {
    background-color: #4EE7C0 !important;
    border-color: #4EE7C0 !important;
    font-size: 18px !important;
    font-family: Pacaembu,sans-serif !important;
    font-weight: 700 !important;
    color: #fff !important;
    text-transform: capitalize !important;
}

.h3-description {
    font-weight: 400;
}

</style>

<template>
    
    <!-- Column Section Starts -->
    
    <section class="column-section" scoped>
        
        <v-div class="cta-img-div" v-for="(item, index) in logoItems" :key="index" variant="outlined" scoped>
            <v-img class="cta-img" :width="500" aspect-ratio="4/3" :src="item.href" scoped></v-img>
        </v-div>
        
        <div scoped>
            
            <h1>Deploy your ratings, globally</h1>
            <h3 class="h3-description"><strong>Skip the painful setup and development.</strong> LevelTech is a global, production-ready system. Skip all the custom dev work and feed your results directly into your ratings.</h3>
            <div>
                <v-btn variant="tonal" scoped>Deploy Now</v-btn>
            </div>
            
        </div>
        
    </section>
    
    <!-- Column Section Starts -->
    
</template>

<script>
import MayaFriends from '@/assets/images/MayaFriends.png';

export default {
    data() {
        return {
            logoItems: [
            { href: MayaFriends },
            ],
        };
    },
};
</script>