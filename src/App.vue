<template>
  <div id="start">
    <HeaderComp/>
    <MainComp/>
</div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'


export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp
  }
}
</script>
<style lang="scss">
#start {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#start > img {
width: 150px;
height: 150px;
padding: 20px 20px;
}
* {
margin: 0 auto;
padding: 0;
box-sizing: border-box;
}
</style>

