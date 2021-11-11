<template>
  <svg :style="style">
    <use :href="iconName"></use>
  </svg>
</template>

<script>
export default {
  name: 'Icon',
  props: {
    name: String,
    style: Object,
  },
  setup(ctx) {
    return {
      iconName: `#${ctx.name}`
    }
  }
}
</script>
