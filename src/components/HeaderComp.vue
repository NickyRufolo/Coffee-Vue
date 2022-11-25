<template>
  <header>
    <div class="img-div">
      <img src="./startbux.jpeg" alt="">
    </div>
  <div class="list">
    <div>
      <a href="#">OUR COFFEE</a>
    </div>
    <div>
      <a href="#">APP</a>
    </div>
    <div>
      <a href="#">TRY</a>
    </div>
    <div>
      <a href="#">OUR CULTURE</a>
    </div>
    <div>
      <a href="#">CONTACTS</a>
    </div>
  </div>
</header>
</template>

<script>
export default {
  name: 'HeaderComp',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">

#start > img {
width: 150px;
height: 150px;
padding: 20px 20px;
}

header {
background-color: whitesmoke;
display: flex;
align-items: center;
}
.list {
display: flex;
gap: 15px;
padding-right: 15px;
}

.list div a {
  color: #006600;
  text-decoration: none;
  font-size:larger;
  font-family: sans-serif;
}
.img-div > img{
width: 100px;
}
</style>

