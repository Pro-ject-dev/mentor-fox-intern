<template>

    <appbar />
    <imge />
    <secondary/>
    <spec/>
    <scrren4/>

</template>

<script>
import imge from './components/image_slider.vue'
import appbar from './components/appbar.vue'
import secondary from './components/secondary.vue'
import spec from './components/specifications.vue'
import scrren4 from './components/screen_4.vue'

export default {
  name: 'app',
  components: {
    appbar,
    imge,
    secondary,
    spec,
    scrren4

  },
}
</script>

<style>
* {
  padding: 0px;
  margin: 0px;
  box-sizing: border-box;
}
</style>
