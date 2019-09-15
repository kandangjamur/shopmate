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
      <section class="promo mt-6">
      </section>
    </div>
  </div>
</template>

<script>
import ComponentFilter from '@/components/list-filter'
import CardItem from '@/components/card'
export default {
  components: {
    ComponentFilter,
    CardItem
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

.shop-listing .item:not(:nth-child(3n+0)) {
  padding-right: 20px;
  margin-bottom: 20px;
}

.recomendations .item:not(:nth-child(3n+0)) {
  padding-right: 30px;
}
</style>
