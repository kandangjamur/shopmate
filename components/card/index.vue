<template>
  <div
    class="card-item relative bg-white cursor-pointer"
    :class="isHover ? 'shadow-2xl' : 'shadow'"
    @mouseenter="isHover = true"
    @mouseleave="isHover = false"
  >
    <div
      v-if="specialLabel !== ''"
      class="special-label text-lg font-bold text-white red-bg inline absolute"
    >
      {{ specialLabel }}
    </div>

    <!-- <div class="overlay-item absolute" :class="isHover ? 'block': 'hidden'" /> -->

    <div class="image px-6 pt-6">
      <img class="block m-auto" src="@/assets/images/images-shirt5.png" alt="Item-image">
    </div>
    <div class="body px-6 pt-4 pb-6 text-center">
      <h4 class="text-lg font-bold">
        Men's Knitwear Offers
      </h4>
      <div class="text-lg mt-3 mb-4">
        <ButtonBase label="Buy Now" onClick="" />
      </div>
    </div>
  </div>
</template>

<script>
import ButtonBase from '@/components/button/base'
export default {
  name: 'CardItem',
  components: {
    ButtonBase
  },
  props: {
    cardType: { type: String, default: 'default' },
    specialLabel: { type: String, default: '' },
    buttonOnClick: { type: Function, default: () => {} }
  },
  data () {
    return {
      isHover: false
    }
  }
}
</script>

<style scoped>
  .cart-item {
    width: 100%;
    background: #ffffff;
  }

  .image img {
    height: 240px;
  }

  .overlay-item {
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: #ffffff;
    opacity: 0.9;
  }

  .special-label {
    padding: 2px 9px;
    top: 10px;
    left: 10px;
    letter-spacing: 2px;
    padding-top: 4px;
  }
</style>
