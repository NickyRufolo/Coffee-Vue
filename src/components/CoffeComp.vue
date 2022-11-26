<template>
    <div class="coffee-card">
        <img :src="propsCoffe.image" alt="">
        <h2>{{propsCoffe.title}}</h2>
    </div>
    </template>
    
    
    
    <script>
    export default {
        name: 'CoffeComp',
        props: {
            propsCoffe : Object
        }
    }
    </script>
    
    <!-- Add "scoped" attribute to limit CSS to this component only -->
    <style scoped lang="scss">
    .coffee-card {
    width: calc(( 100% / 6 ) - 20px );
    border: 1px solid rgb(12, 131, 52);
    text-align: center;
    margin: 10px 10px;
    background-color:  rgb(12, 131, 52);
    color: white;
    }
    .coffee-card > img {
    width: 100%;
    }
    </style>