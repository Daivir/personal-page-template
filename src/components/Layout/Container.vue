<template>
  <div :class="[ fluid ? 'container-fluid' : 'container' ]">
    <slot/>
  </div>
</template>

<script>
export default {
  name: 'container',
  props: {
    fluid: {
      type: Boolean,
      default: false
    }
  }
}
</script>
