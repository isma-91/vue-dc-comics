<template>
  <main>
    <div class="main-top" />
    <div class="main-middle">
      <div class="container">
        <div class="news">
          <h2>CURRENT SERIES</h2>
        </div>
        <DcCard
          v-for="objComic in arrDcCards"
          :key="objComic.series"
          :comic="objComic"
          class="comic-card"
        />
        <button class="btn-load-more">LOAD MORE</button>
      </div>
    </div>
    <div class="main-bot">
      <div class="container">
        <ul>
          <li>
            <a href="!#"><img src="@/img/buy-comics-digital-comics.png" alt="">digital comics</a>
          </li>
          <li>
            <a href="!#"><img src="@/img/buy-comics-merchandise.png" alt="">dc merchandise</a>
          </li>
          <li>
            <a href="!#"><img src="@/img/buy-comics-subscriptions.png" alt="">subscription</a>
          </li>
          <li>
            <a href="!#"><img src="@/img/buy-comics-shop-locator.png" alt="">comic shop locator</a>
          </li>
          <li>
            <a href="!#"><img src="@/img/buy-dc-power-visa.svg" alt="">dc power visa</a>
          </li>
        </ul>
      </div>
    </div>
  </main>
</template>

<script>
import DcCard from '@/components/DcCard.vue';

export default {
  name: 'MainSection',
  components: {
    DcCard,
  },
  data() {
    return {
      arrDcCards: [
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX',
          price: '$19.99',
          series: 'Action Comics',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01',
          price: '$3.99',
          series: 'American Vampire 1976',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb',
          price: '$16.99',
          series: 'Aquaman',
          type: 'graphic novel',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76',
          price: '$2.99',
          series: 'Batgirl',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
          price: '$3.99',
          series: 'Batman',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
          price: '$2.99',
          series: 'Batman Beyond',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8',
          price: '$3.99',
          series: 'Batman/Superman',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk',
          price: '$4.99',
          series: 'Batman/Superman Annual',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8',
          price: '$5.99',
          series: 'Batman: The Joker War Zone',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY',
          price: '$6.99',
          series: 'Batman: Three Jokers',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX',
          price: '$4.99',
          series: 'Batman: White Knight Presents: Harley Quinn',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq',
          price: '$16.99',
          series: 'Catwoman',
          type: 'graphic novel',
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>

.container {
  display: flex;
  flex-wrap: wrap;
  width: 1200px;
  height: 100%;
  margin: auto;
  position: relative;
}

.main-top {
  background-image: url('@/img/jumbotron.jpg');
  background-position: top;
  background-size: cover;
  background-repeat: no-repeat;
  min-height: 600px;
  color: white;
  padding: 3rem 0;
}

.main-middle {
background-color: #1C1C1C;
  .container {

    padding: 4rem 0;
    gap: 2rem;
  }
  .comic-card {
    flex: 0 1 auto;
    width: calc((100% - 2rem * 5) / 6);
  }

  .comic-card:hover {
  transform: translateY(-20px);
  transition: 0.4s ease-out;
  }
  .news {
    background-color: #0282F9;
    color: white;
    height: max-content;
    position: absolute;
    padding: .7rem;
    bottom: 96%;
    left: 0;
  }
  .btn-load-more{
    background-color: #0282F9;
    color: white;
    cursor: pointer;
    border: none;
    margin: auto;
    padding: .7rem 3rem;
    font-weight: bold;
  }

  .btn-load-more:hover {
    filter: brightness(1.2);
  }
}

.main-bot {
  background-color: #0282F9;
  color: white;
  text-transform: uppercase;
  padding: 3rem;
}

.main-bot img {
  height: 40px;
  margin-right: .5rem;
}

.main-bot ul {
  display: flex;
  justify-content: space-around;
  width: 100%;
}

.main-bot li {
  display: flex;
  align-items: center;
}

.main-bot a:hover {
  transition: all .5s linear;
  transform: scale(1.2);
}
</style>
