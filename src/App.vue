<template>
  <div id="app">
    <HeaderComics/>
    <WallpaperComics/>
    <JumbotronComics/>
    <IconsComics/>
    <LinksComics/>
    <FooterComics/>
  </div>
</template>

<script>
import HeaderComics from './components/HeaderComics.vue'
import JumbotronComics from './components/JumbotronComics.vue'
import IconsComics from './components/IconsComics.vue'
import LinksComics from './components/LinksComics.vue'
import FooterComics from './components/FooterComics.vue'
import WallpaperComics from './components/WallpaperComics.vue'

export default {
  name: 'App',
  components: {
    HeaderComics,
    JumbotronComics,
    IconsComics,
    LinksComics,
    FooterComics,
    WallpaperComics
  }
}
</script>

<style lang="scss">
* {
  font-family: Arial, Helvetica, sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
