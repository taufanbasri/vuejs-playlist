<template>
  <div>
    <app-header :title="title"></app-header>
    <app-ninjas :ninjas="ninjas"></app-ninjas>
    <app-footer :title="title"></app-footer>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Ninjas from './components/Ninjas.vue'
import Footer from './components/Footer.vue'

export default {
  components: {
    'app-header': Header,
    'app-ninjas': Ninjas,
    'app-footer': Footer
  },
  data () {
    return {
      ninjas: [
          { name: 'Ryu', speciality: 'Vue Components', show: false },
          { name: 'Hiroshi', speciality: 'HTML Wizard', show: false },
          { name: 'Yoshi', speciality: 'Data Diggin', show: false }
      ],
      title: "Vue Ninjas"
    }
  }
}
</script>

<style>

</style>
