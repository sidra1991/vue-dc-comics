<template>
  <div class="hello">
    <header>
      <div class="header-left">
        <img alt="Vue logo" src="../assets/img/dc-logo.png">
      </div>
      <div class="header-right" >
        <ul>
          <li v-for="(links,index) in list" :key="index" ><a href="#">{{list[index].address}}</a></li>
        </ul>
      </div>
    </header>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      list: [{
        address: 'CHARACTERS',
        link: '#'
      },
      {
        address: 'COMICS',
        link: '#'
      },
      {
        address: 'MOVIE',
        link: '#'
      },
      {
        address: 'TV',
        link: '#'
      },
      {
        address: 'GAMES',
        link: '#'
      },
      {
        address: 'COLLECTIBLES',
        link: '#'
      },
      {
        address: 'VIDEOS',
        link: '#'
      },
      {
        address: 'FANS',
        link: '#'
      },
      {
        address: 'NEWS',
        link: '#'
      },
      {
        address: 'SHOP',
        link: '#'
      }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  background-color: white;
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
