<template>
  <button
    class="button-base font-bold py-2 px-4"
    :style="{ 'color': color, 'background': background }"
  >
    {{ label }}
  </button>
</template>

<script>
export default {
  name: 'ButtonBase',
  props: {
    label: { type: String, default: 'Button Base' },
    onClick: { type: Function, default: () => {} },
    color: { type: String, default: '#ffffff' },
    background: { type: String, default: '#e9425c' },
    buttonType: { type: String, default: 'default' } // in default or light
  }
}
</script>

<style scoped>
.button-base {
  border-radius: 25px;
}

button:active,
button:focus {
  outline: none;
}

button:active {
  background: #a72e41!important;
}
</style>
