<template>
  <v-app>
    <!-- nav goes here -->
    <v-main>
      <nuxt />
    </v-main>
    <app-footer />
  </v-app>
</template>

<script>
export default {
  components: {
    AppFooter: () => import('~/components/layout/AppFooter.vue')
  }
}
</script>

<style></style>
