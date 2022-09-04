<template>

<div>
    <h1>This is my Form</h1>
    {{2+2}}
</div>

<navbar-vue></navbar-vue>
<content-vue></content-vue>
<footer-vue></footer-vue>

</template>

<script>

import navbarVue from './components/navbar.vue';
import footerVue from './components/footer.vue';
import contentVue from './components/content.vue';

export default {

  
    name: 'App',
    components: {
    navbarVue,
    footerVue,
    contentVue

  
}
}
</script>



<style>
</style>