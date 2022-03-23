<template>
  <div class="blue-line">
    <ul>
      <li v-for="(links,index) in list" :key="index"  > <img :src="list[index].address" :alt="list[index].content"> <a :href="list[index].link">{{list[index].content}}</a> </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'BlueLine',
  data () {
    return {
      list: [{
        address: '../assets/img/buy-comics-digital-comics.png',
        content: 'DIGITAL COMICS',
        link: '#'
      },
      {
        address: '../assets/img/buy-comics-digital-comics.png',
        content: 'DC MERCHANDISE',
        link: '#'
      },
      {
        address: '../assets/img/buy-comics-digital-comics.png',
        content: 'SUBSCRIPTION',
        link: '#'
      },
      {
        address: '../assets/img/buy-comics-digital-comics.png',
        content: 'COMIC SHOP LOCATOR',
        link: '#'
      },
      {
        address: '../assets/img/buy-comics-digital-comics.png',
        content: 'DC POWER VISA',
        link: '#'
      }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .blue-line {
    height: 100px;
    background-color: #0282f9;
    ul{
      height: 100%;
      display: flex;
      align-items: center;
      justify-content: center;
      li{
        display: flex;
        flex-wrap: nowrap;
        align-items: center;
        img{
          width: 50px;
          margin-right: 0.5rem ;
        }
        a {
          text-decoration: none;
          color: white;
        }
      }
    }
  }
</style>
