<template>

    <appbar />
    <imge />
    <secondary/>
    <spec/>
    <scrren4/>
    <screen5/>
    <screen6/>
    <screen7/>
<fotter/>
</template>

<script>
import imge from './components/image_slider.vue'
import appbar from './components/appbar.vue'
import secondary from './components/secondary.vue'
import spec from './components/specifications.vue'
import scrren4 from './components/screen_4.vue'
import screen5 from './components/screen_5.vue'
import screen6 from './components/screen_6.vue'
import screen7 from './components/screen_7.vue'
import fotter from './components/footer.vue'
export default {
  name: 'app',
  components: {
    appbar,
    imge,
    secondary,
    spec,
    scrren4,
    screen5,
    screen6,
    screen7,
    fotter

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
