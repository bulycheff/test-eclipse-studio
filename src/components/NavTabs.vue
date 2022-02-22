<template>
  <div class="nav-tabs">
    <v-tabs>
      <v-tab
          @click.prevent="$router.replace(`${tab.path}`)"
          v-for="tab in tabs"
          :key="tab.path"
      >
        {{ tab.name }}
      </v-tab>
    </v-tabs>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      tabs: [
        { name: 'Список валют', path: '/currencies' },
        { name: 'Список валют', path: '/converter' }
      ]
    }
  },
}
</script>

<style>
.nav-tabs {
  margin-bottom: 30px;
}
</style>
