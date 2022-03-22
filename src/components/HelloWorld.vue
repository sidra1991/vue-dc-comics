<template>
  <div class="hello">
    <header>
      <div class="header-left">
        <img alt="Vue logo" src="../assets/img/dc-logo.png">
      </div>
      <div class="header-right" >
        <ul>
          <li><a href="#">CHARACTERS</a></li>
          <li><a href="#"> COMICS </a></li>
          <li><a href="#"> MOVIE </a></li>
          <li><a href="#"> TV </a></li>
          <li><a href="#"> GAMES </a></li>
          <li><a href="#"> COLLECTIBLES</a> </li>
          <li><a href="#"> VIDEOS </a></li>
          <li><a href="#"> FANS </a></li>
          <li><a href="#"> NEWS </a></li>
          <li><a href="#"> SHOP </a></li>
        </ul>
      </div>
    </header>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  margin-top: 20px;
  display: flex;
  margin-top: 0;
  height: 100px;
  width: 100%;
}

.header-left{
  width: 50%;
  height: 100%;
  text-align: center;
}

.header-right {
  overflow: hidden;
  height: 100%;
  ul{
    height: 100%;
    li{
      height: 100%;
      display: inline-block;
      margin: 0.2rem;
      position: relative;
      a{
        line-height: 100px;
        display: inline-block;
        height: 95%;
        text-decoration: none;
        color: black;
        border-bottom: 3px solid transparent;
        &:hover{
          color:blue;
          border-bottom:3px solid blue;
        }
      }
    }
  }
}

img {
  width: 100px;
}

</style>
