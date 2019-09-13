<template>
  <div class="shop-header">
    <!-- top -->
    <div class="header-top">
      <div class="wrapper flex justify-between py-5">
        <div class="nav-item flex items-center">
          <h4 class="flex font-bold pr-1">
            <p class="pr-1">
              Hi!
            </p>
            <ButtonLink
              to="/sign-in"
              label="Sign In"
              color="#e9425c"
            />
          </h4>

          <h4 class="flex font-bold">
            <p class="pr-1">
              or
            </p>
            <ButtonLink
              to="/register"
              label="Register"
              color="#e9425c"
            />
          </h4>
        </div>

        <div class="nav-item flex items-center">
          <div class="menu-item pr-6">
            <h4 class="font-bold">
              <ButtonLink to="/daily-deals" label="Daily Deals" />
            </h4>
          </div>

          <div class="menu-item pr-6">
            <h4 class="font-bold">
              <ButtonLink to="/sell" label="Sell" />
            </h4>
          </div>

          <div class="menu-item">
            <h4 class="font-bold">
              <ButtonLink to="/support" label="Help & Contact" />
            </h4>
          </div>
        </div>

        <div class="nav-item flex items-center">
          <img class="pr-1" src="@/assets/icons/gbr.png" alt="Flag">
          <h4 class="font-bold">
            &euro; GBP
          </h4>
        </div>

        <div class="nav-item flex items-center">
          <Cart count="6" countBg="#e9425c" />
          <h4 class="font-bold pl-4">
            Your bag: &euro; 3.99
          </h4>
        </div>
      </div>
    </div>

    <!-- bottom -->
    <div class="header-bottom black-bg">
      <div class="wrapper flex justify-between py-4">
        <div class="nav-item brand items-center">
          <h2 class="red-color font-bold text-2xl">
            <ButtonLink
              to="/"
              label="S H O P M A T E"
            />
          </h2>
        </div>

        <div class="nav-item flex items-center">
          <div class="menu-item">
            <h4 class="font-bold pr-6">
              <ButtonLink
                to="/category/woman"
                label="Women"
                color="#ffffff"
              />
            </h4>
          </div>

          <div class="menu-item">
            <h4 class="font-bold pr-6">
              <ButtonLink
                to="/category/men"
                label="Men"
                color="#ffffff"
              />
            </h4>
          </div>

          <div class="menu-item">
            <h4 class="font-bold pr-6">
              <ButtonLink
                to="/category/kids"
                label="Kids"
                color="#ffffff"
              />
            </h4>
          </div>

          <div class="menu-item">
            <h4 class="font-bold pr-6">
              <ButtonLink
                to="/category/shoes"
                label="Shoes"
                color="#ffffff"
              />
            </h4>
          </div>

          <div class="menu-item">
            <h4 class="font-bold pr-6">
              <ButtonLink
                to="/category/brands"
                label="Brands"
                color="#ffffff"
              />
            </h4>
          </div>
        </div>

        <div class="nav-item flex items-center">
          <div class="item pr-3">
            <Search />
          </div>

          <div class="item">
            <Cart count="6" cartType="light" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ButtonLink from '@/components/button/link'
import Cart from '@/components/cart/icon'
import Search from '@/components/input/search'
export default {
  name: 'Header',
  components: {
    ButtonLink,
    Cart,
    Search
  }
}
</script>

<style scoped>
  .brand .button-link:hover {
    text-decoration: none;
  }
</style>
