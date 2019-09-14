<template>
  <button class="button-base">
    {{label}}
  </button>
</template>

<script>
export default {
  name: 'ButtonBase',
  props: {
    label: { type: String },
    onClick: { type: Function }
  }
}
</script>

