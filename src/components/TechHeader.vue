<template>

<div class="tech_header">

<div>
<img alt="Vue logo" class="tech_logo" src="../assets/images/logo.svg" width="125" height="125" />
</div>

<div class="tech_cta">

<div>
<v-list :items="items"></v-list>
</div>

<div>
<v-btn prepend-icon="mdi-vuetify" variant="outlined">Button</v-btn>

</div>

</div>

</div>

</template>

<script>
export default {
data: () => ({
items: [
{
title: 'Item #1',
value: 1,
},
{
title: 'Item #2',
value: 2,
},
{
title: 'Item #3',
value: 3,
},
],
}),
}
</script>