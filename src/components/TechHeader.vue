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

</style>

<template>

    <!-- Header Starts -->
  
    <div class="tech_header">

      <!-- Logo Starts Here -->
      <div>
        <img alt="Vue logo" class="tech_logo" src="../assets/images/logo.svg" width="125" height="125" />
      </div>
      <!-- Logo Starts Here -->
  
      <!-- CTA's Starts Here -->
      <div class="tech_cta">

        <!-- Menu Starts Here -->
        <div class="tech_menu">

          <v-menu open-on-hover>
            <template v-slot:activator="{ props }" scoped>
              <v-btn variant="plain" append-icon="mdi-chevron-down" v-bind="props">Platform</v-btn>
            </template>
            <v-list scoped>
              <v-list-item v-for="(item, index) in platformItems" :key="index" scoped>
                <v-list-item-title tag="a" v-bind:href="item.href" scoped>{{ item.title }}</v-list-item-title>
              </v-list-item>
            </v-list>
          </v-menu>

          <v-btn variant="plain">Integrations</v-btn>

          <v-menu open-on-hover>
            <template v-slot:activator="{ props }">
              <v-btn variant="plain" append-icon="mdi-chevron-down" v-bind="props">Solutions</v-btn>
            </template>
            <v-list scoped>
              <v-list-item v-for="(item, index) in solutionItems" :key="index">
                <v-list-item-title tag="a" v-bind:href="item.href">{{ item.title }}</v-list-item-title>
              </v-list-item>
            </v-list>
          </v-menu>

          <v-btn variant="plain">Docs</v-btn>

          <v-btn variant="plain">Pricing</v-btn>
          <!-- Menu Ends Here -->
        
        </div>
        <!-- Cta Button Starts -->
        
        <div>
          <v-btn prepend-icon="mdi-finance" variant="outlined">Get Started</v-btn>
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
        { title: 'Click Us', href: 'https://www.squashlevels.com/' },
        { title: 'Click Us', href: 'https://www.squashlevels.com/' },
        { title: 'Click Us', href: 'https://www.squashlevels.com/' },
        { title: 'Click Us', href: 'https://www.squashlevels.com/' },
      ],
      solutionItems: [
        { title: 'Click Me', href: 'https://www.squashlevels.com/' },
        { title: 'Click Me', href: 'https://www.squashlevels.com/' },
        { title: 'Click Me', href: 'https://www.squashlevels.com/' },
        { title: 'Click Me', href: 'https://www.squashlevels.com/' },
      ],
    };
  },
};
</script>