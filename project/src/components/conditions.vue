<template>
    <h2>Conditional</h2>
    <div>
        <button id="btnConditional" @click="showMessage = !showMessage">Click me!</button>
        <p v-if="!showMessage">This is a message with condition</p>
        <p v-else></p>
    </div>
    <h2>List of prices</h2>

    <div class="list" v-for="price of prices" :key="price.id">
        {{ price.price }}</div>
</template>

<script>


export default {

    data() {
        return {
            showMessage: true,
            showList: true,
            prices: [
                { id: 0, price: "19.99" },
                { id: 1, price: "20.50" },
                { id: 2, price: "35.00" },
                { id: 3, price: "65.50" },
            ]
        }
    }
}
</script>


<style>
#btnConditional {
    background-color: blue;
    color: orange;
    border-radius: 10px;
    font-size: 24px;
    cursor: pointer;
    border: 5px solid white;
}

#btnConditional:hover {
    background-color: darkblue;
    color: cyan;
    border: 5px solid red;
}

#btnArray {
    background-color: orange;
    color: blue;
    border-radius: 10px;
    font-size: 24px;
    cursor: pointer;
    border: 5px solid white;
}

#btnArray:hover {
    background-color: darkblue;
    color: cyan;
    border: 5px solid fuchsia;
}

.list{
    display:flex;
    border: 4px solid grey;
    width: 100px;
    justify-content: center;
    font-weight: bold;
    padding: 10px;
}
.list:hover{
    background-color: blue;
    color: white;
    border-radius: 10px;
    border: 4px solid orange;
    cursor:pointer;
}
</style>