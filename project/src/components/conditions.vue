<template>
    <h2>Conditional</h2>
    <div>
        <button @click="showMessage = !showMessage">Click me!</button>
        <p v-if="!showMessage">This is a message with condition</p>
        <p v-else></p>

  
    </div>
</template>

<script>


    export default {
        
        data() {
            return {
                showMessage: true,
            }
        }
    }
</script>


<style>
    button {
        background-color: blue;
        color: white;
        border-radius: 10px;
        font-size: 24px;
        cursor: pointer; 
        border: 5px solid white;
    }
    button:hover {
        background-color: darkblue;
        color: cyan;
        border: 5px solid red;
    }
</style>