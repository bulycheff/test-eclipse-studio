<template>
  <v-container>
    <div id="app">
      <nav-tabs/>
      <router-view/>
    </div>
  </v-container>
</template>

<script>
import NavTabs from './components/NavTabs'

export default {
  components: {
    NavTabs
  }
}

</script>

<style lang="scss">

</style>
