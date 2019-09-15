<template>
  <div class="subscribe relative">
    <img class="absolute" src="@/assets/icons/icons-email-black.png" alt="Icon Search">
    <input
      type="text"
      class="gray-3-color bg-white font-bold shadow"
      placeholder="Your e-mail here"
      @change="(e) => onValueChange(e.target.value)"
    >
  </div>
</template>

<script>
export default {
  name: 'EmailNewsLetter',
  props: {
    onValueChange: { type: Function }
  }
}
</script>

<style scoped>
::-webkit-input-placeholder { /* Chrome/Opera/Safari */
  color: #bababa;
  }

  ::-moz-placeholder { /* Firefox 19+ */
    color: #bababa;
  }

  :-ms-input-placeholder { /* IE 10+ */
    color: #bababa;
  }

  :-moz-placeholder { /* Firefox 18- */
    color: #bababa;
  }

  input:focus,
  input:active {
    outline: none;
  }

  .subscribe input {
    padding: 10px 15px 10px 50px;
    min-width: 350px;
    border-radius: 25px;
  }

  img {
    width: 25px;
    height: 25px;
    top: 50%;
    transform: translateY(-50%);
    left: 18px;
    object-fit: cover;
  }

  img.close {
    right: 8px;
    left: unset;
    width: 30px;
  }
</style>
