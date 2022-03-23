<template>
  <div class="blue-line">
    <ul>
      <li v-for="(links,index) in list" :key="index"  > <img v-if=" list[index].address != '' " :src="list[index].address" :alt="list[index].content"> <div class="svg" v-if=" list[index].address == '' " >{{list[index].alternative}}</div>  <a :href="list[index].link">{{list[index].content}}</a> </li>
    </ul>
  </div>
</template>

<script>
import digitalComicsImageSquare from '../assets/img/buy-comics-digital-comics.png'
import digitalComicsImageshirt from '../assets/img/buy-comics-merchandise.png'
import digitalComicsImageCard from '../assets/img/buy-comics-subscriptions.png'
import digitalComicsImageGps from '../assets/img/buy-comics-shop-locator.png'
import svgPazza from '../assets/img/buy-dc-power-visa.svg'
export default {
  name: 'BlueLine',
  data () {
    return {
      list: [{
        address: digitalComicsImageSquare,
        content: 'DIGITAL COMICS',
        link: '#'
      },
      {
        address: digitalComicsImageshirt,
        content: 'DC MERCHANDISE',
        link: '#'
      },
      {
        address: digitalComicsImageCard,
        content: 'SUBSCRIPTION',
        link: '#'
      },
      {
        address: digitalComicsImageGps,
        content: 'COMIC SHOP LOCATOR',
        link: '#'
      },
      {
        address: '',
        alternative: svgPazza,
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
