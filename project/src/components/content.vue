<template>
    <div>
        <h2>Content component</h2>
        <p>{{ property }}</p>
    </div>

</template>

<script>
export default {
    data() {
        return {
            property: '',
        };
    },

    computed: {
        propertyComputed() {

            console.log('I change when this.property changes.');

            return this.property;
        },


    },

    created() {

        this.property = 'Example property update.'
        console.log('propertyComputed will update, as this.property is now reactive.')

    }
}

</script>

<style>
</style>