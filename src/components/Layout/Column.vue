<template lang="html">
  <div class="column" :class="classObject">
    <slot/>
  </div>
</template>

<script>
export default {
  name: 'column',
  props: {
    xs: {
      type: String,
      default: '12'
    },
    sm: String,
    md: String,
    lg: String
  },
  computed: {
    classObject () {
      let classes = Object.keys(this.$props).map((key) => {
        let value = this.$props[key]
        if (typeof value === 'string') return key + value
      }, this)
      return classes.join(' ').trim()
    }
  }
}
</script>
