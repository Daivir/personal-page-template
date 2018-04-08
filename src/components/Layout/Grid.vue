<template>
  <div class="grid" :class="classObject">
    <slot/>
  </div>
</template>

<script>
export default {
  name: 'grid',
  props: {
    row: Boolean,
    column: Boolean,
    reverse: Boolean,
    wrap: Boolean
  },
  computed: {
    classObject () {
      let classes = Object.keys(this.$props).filter((key) => {
        let value = this.$props[key]
        if (value && typeof value === 'boolean') return key
      }, this)
      return classes.join(' ').trim()
    }
  }
}
</script>
