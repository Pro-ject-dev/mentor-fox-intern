<template>
    <appbar />
    <home />
    <secondary/>
    <rooms/>
    <features/>
    <customers/>
    <consultation/>
    <help/> 
    <footers/>
</template>

<script>
import appbar from './components/appbar.vue'
import home from './components/landing_page/home.vue'
import secondary from './components/story_screen/secondary.vue'
import rooms from './components/specification/rooms.vue'
import features from './components/features/features.vue'
import customers from './components/customers/customers.vue'
import consultation from './components/consultation/consultation.vue'
import help from './components/help/help.vue'
import footers from './components//footer/footer.vue'
export default {
  name: 'app',
  components: {
    appbar,
    home,
    secondary,
    rooms,
    features,
    customers,
    consultation,
    help,
    footers

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
