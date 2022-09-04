<template>

<div>
    <h1>Exercise with components</h1>
    {{2+2}}
</div>

<navbar-vue></navbar-vue>
<content-vue></content-vue>
<conditions-vue></conditions-vue>
<footer-vue></footer-vue>

</template>

<script>

import navbarVue from './components/navbar.vue';
import contentVue from './components/content.vue';
import conditionsVue from './components/conditions.vue';
import footerVue from './components/footer.vue';



export default {

  
    name: 'App',
    components: {
    navbarVue,
    contentVue,
    conditionsVue,
    footerVue,
    

  
}
}
</script>



<style>
</style>