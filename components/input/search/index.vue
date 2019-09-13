<template>
  <div class="search relative">
    <img class="absolute" src="@/assets/icons/icons-search-white.png" alt="Icon Search">
    <img class="cursor-pointer absolute close" src="@/assets/icons/icons-close-small-white.png" alt="Icon Close">
    <input
      type="text"
      class="text-white gray-bg font-bold"
      placeholder="search anything"
      @change="(e) => onValueChange(e.target.value)"
    >
  </div>
</template>

<script>
export default {
  name: 'Search',
  props: {
    onValueChange: { type: Function }
  }
}
</script>

<style scoped>
  ::-webkit-input-placeholder { /* Chrome/Opera/Safari */
  color: #ffffff;
  }

  ::-moz-placeholder { /* Firefox 19+ */
    color: #ffffff;
  }

  :-ms-input-placeholder { /* IE 10+ */
    color: #ffffff;
  }

  :-moz-placeholder { /* Firefox 18- */
    color: #ffffff;
  }

  input:focus,
  input:active {
    outline: none;
  }

  .search input {
    padding: 10px 15px 10px 40px;
    min-width: 350px;
    border-radius: 25px;
  }

  img {
    width: 25px;
    height: 25px;
    top: 50%;
    transform: translateY(-50%);
    left: 9px;
    object-fit: cover;
  }

  img.close {
    right: 8px;
    left: unset;
    width: 30px;
  }
</style>
