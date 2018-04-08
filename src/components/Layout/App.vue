<template>
  <div id="app">
    <header>
      <slot name="header"/>
    </header>
    <slot/>
    <footer>
      <slot name="footer"/>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style lang="stylus">
  *
    outline-offset -1px
    outline 1px solid red
    margin 0
    padding 0
    box-sizing border-box

  html
    scroll-behavior smooth
</style>
