<style scoped>

.v-list {
  --indent-padding: 0px;
  display: flex;
  gap: 0px !important;
  padding: 5%;
  flex-direction: column;
  min-width: 200px;
}
.v-list-item {
  align-items: center;
  display: grid;
  flex: none;
  min-height: 0px;
  grid-template-areas: "prepend content append";
  grid-template-columns: max-content auto max-content;
  outline: none;
  max-width: 100%;
  position: relative;
  text-decoration: none;
  border-color: rgba(var(--v-border-color), var(--v-border-opacity));
  border-style: solid;
  border-width: 0;
  border-radius: 0;
  padding: 7px 12px !important;
}

.v-menu .v-overlay__content {
  display: flex;
  flex-direction: column;
  border-radius: 20px;
}

.v-list-item--density-default.v-list-item--one-line {
  min-height: 0px;
}

.menu_title {
  color: #000 !important;
  font-weight: 700;
  font-family: 'Mulish', sans-serif;
}


.header_cta {
  border-width: 0px;
  border-radius: 5px;
  border-color: #4EE7C0;
  background-color: #4EE7C0;
  color: #fff;
  font-weight: 700;
  font-family: 'Mulish', sans-serif;
}

.v-list-item-title {
  color: #000;
  transition: color 0.2s ease-in-out;
}

.v-list-item-title:hover {
  color: #4EE7C0;
}


</style>

<template>
  
  <!-- Header Starts -->
  
  <div class="tech_header">
    
    <!-- Logo Starts Here -->
    <div>
      <img alt="Vue logo" class="tech_logo" src="../../assets/images/main-logo-light.svg" width="300" height="300" />
    </div>
    <!-- Logo Starts Here -->
    
    <!-- CTA's Starts Here -->
    <div class="tech_cta">
      
      <!-- Menu Starts Here -->
      <div class="tech_menu">
        
        <v-menu open-on-hover>
          <template v-slot:activator="{ props }" scoped>
            <v-btn color="tertiary" variant="plain" append-icon="mdi-chevron-down" v-bind="props" class="menu_title">Platform</v-btn>
          </template>
          <v-list scoped>
            <v-list-item v-for="(item, index) in platformItems" :key="index" scoped>
              <v-list-item-title tag="a" v-bind:href="item.href" scoped>{{ item.title }}</v-list-item-title>
            </v-list-item>
          </v-list>
        </v-menu>
        
        <v-btn variant="plain" class="menu_title" style="color: black;">Integrations</v-btn>
        
        <v-menu open-on-hover>
          <template v-slot:activator="{ props }">
            <v-btn variant="plain" append-icon="mdi-chevron-down" v-bind="props" class="menu_title" style="color: black;">Solutions</v-btn>
          </template>
          <v-list scoped>
            <v-list-item v-for="(item, index) in solutionItems" :key="index">
              <v-list-item-title tag="a" v-bind:href="item.href">{{ item.title }}</v-list-item-title>
            </v-list-item>
          </v-list>
        </v-menu>
        
        <v-btn color="secondary" variant="plain" class="menu_title" href="https://api-docs.surecart.com/">Docs</v-btn>
        
        <v-btn color="secondary" variant="plain" class="menu_title" href="https://draftbit.com/pricing">Pricing</v-btn>
        <!-- Menu Ends Here -->
        
      </div>
      <!-- Cta Button Starts -->
      
      <div>
        <v-btn prepend-icon="mdi-finance" variant="tonal" class="header_cta" scoped>Get Started</v-btn>
      </div>
      <!-- Cta Button Ends -->
      
    </div>
    <!-- CTA's End Here -->
    
  </div>
  
  <!-- Header Ends -->
  
</template>

<script>
export default {
  data() {
    return {
      platformItems: [
      { title: 'Rating System', href: 'https://www.squashlevels.com/' },
      { title: 'Box Leagues', href: 'https://www.squashlevels.com/' },
      { title: 'Global Rankings', href: 'https://www.squashlevels.com/' },
      { title: 'Communities', href: 'https://www.squashlevels.com/' },
      ],
      solutionItems: [
      { title: 'Governance', href: 'https://www.squashlevels.com/' },
      { title: 'Counties', href: 'https://www.squashlevels.com/' },
      { title: 'Clubs', href: 'https://www.squashlevels.com/' },
      { title: 'Players', href: 'https://www.squashlevels.com/' },
      ],
    };
  },
};

window.addEventListener('scroll', function() {
  var header = document.querySelector('header');
  var scrollPosition = window.pageYOffset;
  
  if (scrollPosition > 0) {
    header.classList.add('box-shadow');
  } else {
    header.classList.remove('box-shadow');
  }
});
</script>