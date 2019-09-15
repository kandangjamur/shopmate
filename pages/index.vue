<template>
  <div class="homepage grey-bg">
    <div class="wrapper py-6">
      <!-- section hero -->
      <section class="hero">
      </section>

      <!-- section listing -->
      <section class="shop-listing flex mt-6">
        <div class="w-3/12">
          <ComponentFilter />
        </div>

        <div class="w-9/12 flex flex-wrap">
          <div class="item w-1/3">
            <CardItem specialLabel="HOT" />
          </div>

          <div class="item w-1/3">
            <CardItem />
          </div>

          <div class="item w-1/3">
            <CardItem />
          </div>

          <div class="item w-1/3">
            <CardItem />
          </div>

          <div class="item w-1/3">
            <CardItem />
          </div>

          <div class="item w-1/3">
            <CardItem />
          </div>
        </div>
      </section>

      <!-- section recomendation -->
      <section class="mt-6 flex recomendations">
        <div class="item w-1/3">
          <CardItem />
        </div>
        <div class="item w-1/3">
          <CardItem />
        </div>
        <div class="item w-1/3">
          <CardItem />
        </div>
      </section>

      <!-- section ads -->
      <section class="promo relative mt-6">
        <div class="content flex justify-start flex-wrap">
          <div class="title w-full">
            <h1 class="font-bold font-playfair text-6xl text-white">
              Converse
            </h1>
          </div>

          <div class="sub-title">
            <h2 class="text-4xl text-white font-bold">
              Explore styles tough enough to
            </h2>

            <h2 class="text-4xl text-white font-bold">
              handle all your workouts
            </h2>

            <div class="button mt-3">
              <ButtonBase
                label="Shop Brand"
                color="#e9425c"
                background="#ffffff"
              />
            </div>
          </div>
        </div>
      </section>
    </div>

    <div class="newsletter grey-2-bg py-4">
      <div class="wrapper flex items-center justify-between">
        <h4 class="font-bold text-lg">SUBSCRIBE FOR SHOP NEWS, UPDATES AND SPECIAL OFFERS</h4>
        <form class="news-input flex items-center">
          <div class="item pr-2">
            <NewsLetterInput />
          </div>
          <div class="item">
            <ButtonBase label="Subscribe" />
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
import ComponentFilter from '@/components/list-filter'
import CardItem from '@/components/card'
import NewsLetterInput from '@/components/input/newsletter'
import ButtonBase from '@/components/button/base'
export default {
  components: {
    ComponentFilter,
    CardItem,
    NewsLetterInput,
    ButtonBase
  },
  head () {
    return {
      title: 'Shopmate'
    }
  }
}
</script>

<style scoped>
.hero {
  height: 500px;
  background: url(../assets/images/Images-modal4.png);
  background-repeat: no-repeat;
  background-size: cover;
}
.promo {
  height: 450px;
  background: url(../assets/images/images-shoe2.png);
  background-repeat: no-repeat;
  background-size: cover;
}

.promo::before {
  content: '';
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  background: #000;
  opacity: 0.38;
}

.promo .content {
  position: absolute;
  top: 40%;
  transform: translateY(-50%);
  left: 100px;
}

.promo h1 {
  letter-spacing: 3px;
}

.promo h2 {
  letter-spacing: 2px;
}

.shop-listing .item:not(:nth-child(3n+0)) {
  padding-right: 20px;
  margin-bottom: 20px;
}

.recomendations .item:not(:nth-child(3n+0)) {
  padding-right: 30px;
}
</style>
