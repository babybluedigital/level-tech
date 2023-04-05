<style scoped>
.bg-white-lighten-1 {
    display: flex;
    flex-direction: row;
    padding: 5% 0%;
    margin: 3% 12% 0% 12%;
    border-top: 1px solid;
    border-color: #e9ebed;
}

.v-row {
    display: flex;
    flex-wrap: wrap;
    flex: 1 1 auto;
    margin: -12px;
    flex-direction: column;
    align-content: center;
    justify-content: center;
    align-items: flex-start;
}

.v-btn--variant-plain {
    color: #000;
    text-transform: capitalize;
    font-weight: 500;
    font-size: 18px;
    font-family: Pacaembu,sans-serif;
    transition: all 0.2s ease-in-out;
    padding-left: 0px;
    margin-left: 0px !important;
}

.v-btn--variant-plain:hover {
    color: #4EE7C0 !important;
}

.v-row h6 {
    padding-bottom: 10px !important;
}

#footer_icons {
    background-color: #4EE7C0 !important;
    padding: 0.3% 0% !important;
    display: flex !important;
    flex-direction: column !important;
    align-items: center;
}

</style>

<template>
    
    <div class="bg-white-lighten-1" scoped>
        <v-row justify="center" no-gutters><h6>Why LevelTech</h6>
            <v-btn
            v-for="link in links"
            :key="link"
            variant="plain"
            class="mx-2"
            >
            {{ link }}
        </v-btn>
    </v-row>
    
    <v-row justify="center" no-gutters><h6>Products</h6>
        <v-btn
        v-for="link in links"
        :key="link"
        variant="plain"
        class="mx-2"
        >
        {{ link }}
    </v-btn>
</v-row>

<v-row justify="center" no-gutters><h6>Learn</h6>
    <v-btn
    v-for="link in links"
    :key="link"
    variant="plain"
    class="mx-2"
    >
    {{ link }}
</v-btn>
</v-row>

<v-row justify="center" no-gutters><h6>Company</h6>
    <v-btn
    v-for="link in links"
    :key="link"
    variant="plain"
    class="mx-2"
    >
    {{ link }}
</v-btn>
</v-row>

</div>

<br>

<v-row
class="bg-indigo-lighten-1 text-center d-flex flex-column" id="footer_icons"
>

<v-col class="text-center mt-4" cols="12">
        <strong>© LevelTech</strong>
    </v-col>

<div>
    <v-btn
    v-for="icon in icons"
    :key="icon"
    class="mx-4"
    :icon="icon"
    variant="text"
    ></v-btn>
</div>

<v-divider></v-divider>

</v-row>

</template>

<script>
export default {
    data: () => ({
        links: [
        'Home',
        'About Us',
        'Team',
        'Services',
        'Blog',
        'Contact Us',
        ],
        icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
        ],
    }),
}


</script>   