<template>
  <footer>
    <div class="footer-left" >
      <div class="intro" >
        <ul v-for="(argoment,index) in footerLink" :key="index">{{argoment.title}}
          <li v-for="(links,indexV) in argoment.links" :key="indexV" >
            <a href=""> {{argoment.links[indexV].Concept}} </a>
          </li>
       </ul>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterDc',
  data () {
    return {
      footerLink: [{
        title: 'DC COMICS',
        links: [{
          from: '#',
          Concept: 'Characters'
        },
        {
          from: '#',
          Concept: 'Comics'
        },
        {
          from: '#',
          Concept: 'Movie'
        },
        {
          from: '#',
          Concept: 'Tv'
        },
        {
          from: '#',
          Concept: 'Games'
        },
        {
          from: '#',
          Concept: 'Videos'
        },
        {
          from: '#',
          Concept: 'News'
        }]
      },
      {
        title: 'DC',
        links: [{
          from: '#',
          Concept: 'Term Of Use'
        },
        {
          from: '#',
          Concept: 'Prvacy policy (New)'
        },
        {
          from: '#',
          Concept: 'Ad Choices'
        },
        {
          from: '#',
          Concept: 'Advertising'
        },
        {
          from: '#',
          Concept: 'Jobs'
        },
        {
          from: '#',
          Concept: 'Subscriptions'
        },
        {
          from: '#',
          Concept: 'Talent Workshops'
        },
        {
          from: '#',
          Concept: 'CPSC Certificates'
        },
        {
          from: '#',
          Concept: 'Ratings'
        },
        {
          from: '#',
          Concept: 'Shop help'
        },
        {
          from: '#',
          Concept: 'Contact Us'
        }]
      },
      {
        title: 'SITES',
        links: [{
          from: '#',
          Concept: 'DC'
        },
        {
          from: '#',
          Concept: 'MAD Magazine'
        },
        {
          from: '#',
          Concept: 'DC KIDS'
        },
        {
          from: '#',
          Concept: 'DC Universe'
        },
        {
          from: '#',
          Concept: 'DC Power Visa'
        }]
      },
      {
        title: 'SHOP',
        links: [{
          from: '#',
          Concept: 'Shop DC'
        },
        {
          from: '#',
          Concept: 'Shop DC Collectibles'
        }]
      }]
    }
  }
}
</script>

<style scoped lang="scss">
footer {
  // background-image: url(../assets/img/footer-bg.png);
  height: 600px;
  color: white;
}
.footer-left{
  width: 50%;
  height: 100%;
  .intro{
    margin-left: 40%;
    widows: 50%;
    background-color: wheat;
    display: flex;
    flex-wrap: wrap;
    ul{
      li{
        a{
          color: #959595;
          text-decoration: none;
        }
      }
    }
  }
}
</style>
