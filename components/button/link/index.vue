<template>
  <div
    class="button-link"
    :style="{ 'color': color ? color : ''}"
    @click="$router.push(to)">
    {{ label }}
  </div>
</template>

<script>
export default {
  name: 'ButtonLink',
  props: {
    label: { type: String, default: 'Button Link' },
    to: { type: String, required: true },
    color: { type: String, default: null }
  }
}
</script>

<style scoped>
  .button-link {
    cursor: pointer;
  }

  .button-link:hover {
    text-decoration: underline;
  }
</style>
