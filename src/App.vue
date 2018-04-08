<template>
  <app>
    <container>
      <grid row wrap>
        <column sm=9 md=8 lg=7>
          <section>
            Section
          </section>
        </column>
        <column sm=3 md=4 lg=5>
          <aside>
            Aside
          </aside>
        </column>
      </grid>
      HelloWorld
    </container>
  </app>
</template>

<script>
import components from '@/components'

export default {
  name: 'App',
  components
}
</script>
