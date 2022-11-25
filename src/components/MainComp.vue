<template>
    <main>
        <!-- Pasta -->
        <div class="pre-Coffee">
            <i class="fa-regular fa-square"></i>
            <span class="pastatext">Our <strong>COFFEE</strong></span>
        </div>
        <div class="Pasta-card-Div-Flex">
            <PastaCard v-for="(element, index) in arrayPasta" :key="index" :propsPasta="element" />
        </div>
    </main>
</template>

<script>
export default {
    name: 'MainComp',
    props: {
        msg: String
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
</style> 