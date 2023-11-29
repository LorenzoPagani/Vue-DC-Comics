<script >
import appHeader from './components/appHeader.vue'
import appContent from './components/appContent.vue'
import buyComics from './components/buyComics.vue'
export default {
  components: {
    appHeader,
    appContent,
    buyComics
  }
}
</script>

<template>
  <appHeader />
  <main>
    <appContent />
    <buyComics />
  </main>
</template>

<style scoped></style>
