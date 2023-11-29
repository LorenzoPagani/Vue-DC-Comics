<script >
import appHeader from './components/appHeader.vue'
import appContent from './components/appContent.vue'
import buyComics from './components/buyComics.vue'
import footerMenu from './components/footerMenu.vue'
import callToAction from './components/callToAction.vue'
export default {
  components: {
    appHeader,
    appContent,
    buyComics,
    footerMenu,
    callToAction
  }
}
</script>

<template>
  <appHeader />
  <main>
    <appContent />
    <buyComics />
  </main>
  <footer>
    <footerMenu />
    <callToAction />
  </footer>
</template>

<style scoped></style>
