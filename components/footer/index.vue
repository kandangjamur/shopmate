<template>
  <div class="shop-footer black-bg text-white pt-10 pb-8">
    <div class="footer-wrapper flex items-center justify-between">
      <div class="item">
        <h4 class="font-bold">
          <ButtonLink to="/category/women" label="Women" color="#ffffff" />
        </h4>
      </div>

      <div class="item">
        <h4 class="font-bold">
          <ButtonLink to="/category/men" label="Men" color="#ffffff" />
        </h4>
      </div>

      <div class="item">
        <h4 class="font-bold">
          <ButtonLink to="/category/kids" label="Kids" color="#ffffff" />
        </h4>
      </div>

      <div class="item">
        <h4 class="font-bold">
          <ButtonLink to="/category/shoes" label="Shoes" color="#ffffff" />
        </h4>
      </div>

      <div class="item">
        <h4 class="font-bold">
          <ButtonLink to="/category/brands" label="Brands" color="#ffffff" />
        </h4>
      </div>
    </div>

    <div class="social-footer flex justify-center pt-6">
      <div class="social-item pr-5">
        <img class="cursor-pointer" src="@/assets/icons/icons-instagram-black.png" alt="Icon">
      </div>

      <div class="social-item pr-5">
        <img class="cursor-pointer" src="@/assets/icons/icons-pinterest-black.png" alt="Icon">
      </div>

      <div class="social-item pr-5">
        <img class="cursor-pointer" src="@/assets/icons/icons-twitter-black.png" alt="Icon">
      </div>

      <div class="social-item pr-5">
        <img class="cursor-pointer" src="@/assets/icons/icons-facebook-black.png" alt="Icon">
      </div>
    </div>

    <ul class="company-info flex justify-center gray-2-color mt-6">
      <li class="pr-8 text-lg">
        &copy; 2016 shopmate Ltd
      </li>

      <li class="list-disc pr-8 text-lg">
        Contact
      </li>

      <li class="list-disc text-lg">
        Privacy Policy
      </li>
    </ul>
  </div>
</template>

<script>
import ButtonLink from '@/components/button/link'
export default {
  name: 'Footer',
  components: {
    ButtonLink
  },
  props: {
    footerType: { type: String, default: 'dark' } // in dark and light
  }
}
</script>

<style scoped>
.footer-wrapper {
  max-width: 50%;
  margin: auto;
}
</style>
