<template>

<div>
    <h1>This is my Form</h1>
</div>

<navbar-vue></navbar-vue>
<footer-vue></footer-vue>

</template>

<script>

import navbarVue from './components/navbar.vue';
import footerVue from './components/footer.vue';




export default {
    name: 'App',
    components: {
    navbarVue,
    footerVue
}
}
</script>



<style>
</style>