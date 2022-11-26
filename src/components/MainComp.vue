<template>
    <main>
        <!-- Coffee -->
        <div class="pre-Coffee">
            <i class="fa-regular fa-square"></i>
            <span class="pastatext">Our <strong>COFFEE</strong></span>
        </div>
        <div class="Coffe-card-Div-Flex">
            <CoffeComp v-for="(element, index) in dataCoffe" :key="index" :propsCoffe="element" />
        </div>
    </main>
</template>

<script>
import CoffeComp from "./CoffeComp.vue"
import axios from 'axios'


export default {
    name: 'MainComp',
    components: {
        CoffeComp,
    },
    data() {
        return {
        dataCoffe: ``
        }
    },
    mounted() {
        axios.get(`https://api.sampleapis.com/coffee/hot`)
        .then ((response) => {
            this.dataCoffe = response.data
            // this.dataCoffe = recupero l'info dentro a data
            // response.data.response recupero l'array di tutti i caffe presenti nel response nella chiamata GET dell'api
        })
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
.pre-Coffee {
    width: 80%;
    margin: 30px auto;
    font-size: 1.8rem;
}

.Coffe-card-Div-Flex {
    display: flex;
    width: 80%;
    flex-wrap: wrap;
}
.pre-Coffee i {
    margin-right: 20px;
}
</style> 