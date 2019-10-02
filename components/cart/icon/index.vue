<template>
  <div class="cart relative cursor-pointer">
    <div
      v-if="Number(count) > 0"
      class="count rounded-full absolute
      font-bold flex items-center
      justify-center text-sm"
      :style="{ 'background': countBg }"
      :class="countBg === '#ffffff' ? 'red-color': 'text-white'"
    >
      {{ count }}
    </div>
    <img :src="handleImage" alt="Cart Image">
  </div>
</template>

<script>
import blackImage from '@/assets/icons/icons-bag.png'
import whiteImage from '@/assets/icons/icons-bag-white.png'
export default {
  name: 'Cart',
  props: {
    count: { type: String, default: null },
    countBg: { type: String, default: '#ffffff' },
    cartType: { type: String, default: 'dark' }, // in 'dark' and 'light',
    onClick: { type: Function }
  },
  computed: {
    handleImage () {
      const { cartType } = this
      switch (cartType) {
        case 'dark': {
          return blackImage
        }
        case 'light': {
          return whiteImage
        }
        default: {
          return blackImage
        }
      }
    }
  }
}
</script>

<style scoped>
  .count {
    width: 22px;
    height: 22px;
    top: -10px;
    right: -10px;
  }

  img {
    width: 25px;
    height: 25px;
    object-fit: cover;
  }
</style>
